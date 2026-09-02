# Borscht --- Performance Optimization Guide

S.T.A.L.K.E.R. 2 is a demanding Unreal Engine 5 game. At some point,
almost everyone is going to stare at their FPS counter and wonder where
all their frames wandered off to.

Before installing performance tweaks, replacing DLLs, sacrificing a
Bloodsucker to the Monolith, or blaming Borscht, start with the boring
answer:

> **Establish a stable baseline first. Optimize second. Add expensive
> visual features last.**

------------------------------------------------------------------------

## ☢️ Start With a Clean Performance Baseline

In **Settings → Graphics**, use **Reset Settings** first.

Then compare your hardware against the official GSC system requirements
and choose the appropriate overall graphics preset as your starting
point.

Do not treat **Epic** as the setting you are *supposed* to use. It is
just another quality preset. Your GPU does not care about your feelings.
😄

### Example: RTX 3080 at 1440p

Suppose your system has an Intel Core i9-13700KF, 32 GB DDR5-6600, an
NVIDIA RTX 3080, and an NVMe SSD.

What overall quality preset should you start with for a 1440p / 60 FPS
target?

**High. Not Epic.**

The RTX 3080 is still a capable GPU, but GSC's official **Epic** target
calls for substantially faster hardware such as an RTX 4080. Start from
the preset appropriate to your hardware, establish that the game runs
well, and improve individual settings afterward if you have performance
to spare.

> **Important:** GSC's published performance targets account for modern
> upscaling/frame-generation technologies. They should not be
> interpreted as guaranteed native-resolution performance targets.

------------------------------------------------------------------------

## 🔧 Tune the Expensive Settings First

If the appropriate overall preset is not performing acceptably, do not
immediately reduce every graphics option.

Good first candidates include:

1.  **Rendering Distance**
2.  **Shadows**
3.  **Hair / Foliage**
4.  **Reflections**
5.  **Texture Quality**, particularly when VRAM is limited

If **Rendering Distance** is above Medium and you are struggling, try
Medium and retest.

------------------------------------------------------------------------

## 🧪 Change ONE Thing at a Time

Do **not** change fourteen graphics settings, install three optimization
mods, replace your DLSS DLLs, clear every cache on the computer, change
Windows settings, and then wonder which thing fixed the problem.

Change **one meaningful variable**, test the same area, and compare.

When possible, monitor:

-   FPS
-   1% lows
-   Frame time
-   GPU utilization
-   VRAM utilization
-   CPU utilization
-   CPU/GPU temperatures

Average FPS only tells part of the story. A relatively stable 60 FPS
with consistent frame pacing can feel substantially better than a game
wildly bouncing between 70 and 120 FPS.

------------------------------------------------------------------------

## 🎨 Shader Compilation --- Let It Finish

Yes, Shader Compilation is annoying.

**Let it finish.**

STALKER 2 is doing useful work here. Precompiling shaders allows the
game to prepare GPU programs before you encounter them during gameplay
instead of compiling everything on demand while you are trying to
survive the Zone.

I look at the startup delay as a good excuse to grab some water,
stretch, use the bathroom, get a snack, or question my life choices. ☕

### When Should I Clear the Shader Cache?

**Do not routinely clear your shader cache.**

If it ain't broke, don't fix it.

Clearing the cache can be a useful **advanced troubleshooting step**
when shader compilation appears corrupted, severe graphical problems
suddenly appear after a game or driver update, the game repeatedly
crashes during or immediately after shader initialization, or you have
been specifically instructed to rebuild it.

Clearing the cache forces the game to rebuild it, so expect the next
shader-compilation process to take longer.

------------------------------------------------------------------------

## 💾 VRAM Matters

Unreal Engine 5 can be extremely demanding on VRAM.

One possible symptom of VRAM pressure is a game that initially runs well
but, after playing for a while, deteriorates into a stuttering or
slideshow-like mess.

This is particularly important for otherwise capable older GPUs with 8
GB, 10 GB, or 12 GB of VRAM.

### What to Try

If VRAM is consistently at or near the limit:

1.  Lower **Texture Quality by one step**.
2.  Retest the same location.
3.  Check VRAM usage again.
4.  Only reduce additional settings if necessary.

Do not confuse **GPU utilization** with **VRAM utilization**. They
measure different things.

------------------------------------------------------------------------

## 🖥️ Upscaling

Upscaling is not cheating, nor is it necessarily an emergency
performance hack.

Modern games---including STALKER 2---are designed with technologies such
as **DLSS, FSR, XeSS, and TSR** in mind.

A reasonable progression is:

**Native/DLAA if performance allows → Quality → Balanced → Performance**

Do not automatically select Performance mode just because it produces
the largest FPS number. Lower internal resolutions can noticeably reduce
image quality.

At 1440p, **Quality** is usually a sensible starting point when
upscaling is needed. At 4K, there is more flexibility because the
reconstructed image begins with a much larger pixel budget.

------------------------------------------------------------------------

## 🎞️ Frame Generation

Frame Generation can dramatically increase the displayed frame rate by
inserting generated frames between traditionally rendered frames.

What it **cannot** do is magically transform poor underlying performance
into excellent responsiveness.

### Borscht Rule of Thumb

> 🎯 **Get the game feeling reasonably responsive without Frame
> Generation first. Then enable Frame Generation.**

Think of Frame Generation as the finishing layer---not the foundation
holding everything together.

------------------------------------------------------------------------

## 🔦 Flashlight Artifacts With Frame Generation

Some configurations can exhibit flashlight-related visual artifacts
while Frame Generation is enabled.

A commonly reported workaround is:

> Set **Motion Blur to 1% instead of 0%**.

This effectively keeps visible motion blur negligible while preserving
rendering behavior needed by some Frame Generation configurations.

Treat this as a troubleshooting workaround rather than a mandatory
graphics setting.

------------------------------------------------------------------------

# Borscht-Specific Graphics Advice

Borscht may provide or support a carefully tested graphics stack
including components such as **Ultra+**, ReShade/PRZ, RenoDX,
Streamline, and DLSS-related components.

## ⚠️ Do Not Install Random Engine.ini Performance Tweaks

Borscht's graphics stack is intentionally configured.

Do not assume that an `Engine.ini` advertised as an FPS boost, stutter
fix, UE5 optimization, or input-lag fix belongs in Borscht.

Old Unreal Engine commands, incompatible tweaks, duplicated settings,
and conflicting graphics mods can make performance **worse**, introduce
visual problems, or interfere with Ultra+.

If Borscht's installation instructions tell you that an existing
`Engine.ini` must be removed, **remove it**.

------------------------------------------------------------------------

## ⚠️ Do Not Randomly Swap DLSS or Streamline DLLs

Do not use tools such as **DLSS Swapper**, manually replace DLSS DLLs,
or mix Streamline components unless specifically instructed by the
Borscht documentation.

Borscht may provide specific tested versions of DLSS Super Resolution,
Frame Generation, Ray Reconstruction / Neural Rendering components,
NVIDIA Streamline, and RenoDX integrations.

**Newer does not automatically mean better for this particular
configuration.**

------------------------------------------------------------------------

## ✨ Performance Has a Price

Borscht may include optional visual enhancements because they can make
the Zone look fantastic.

They are still **optional visual enhancements**.

If performance is inadequate:

> **Disable optional visual enhancements before dismantling the
> underlying Borscht installation.**

A midrange GPU cannot reasonably be expected to run every expensive
visual feature at maximum settings simply because the option exists.

------------------------------------------------------------------------

# Optional System Optimization

The following items can be worth checking, but they are **not mandatory
Borscht requirements**.

## 🧠 XMP / EXPO

If your motherboard and memory support **XMP** or **EXPO**, verify that
your memory is actually operating at its intended speed.

> **Stability comes first.**

An unstable XMP/EXPO profile is worse than slightly slower memory.

------------------------------------------------------------------------

## 🧩 Resizable BAR

If supported by your CPU, motherboard, BIOS, and GPU, **Resizable BAR**
can be worth enabling.

Do not expect a universal percentage improvement. The benefit varies by
game and hardware configuration.

------------------------------------------------------------------------

## 🪟 Hardware-Accelerated GPU Scheduling (HAGS)

HAGS can affect latency, scheduling behavior, and Frame Generation
support depending on the GPU, driver, and Windows version.

For modern systems using Frame Generation, it is worth ensuring HAGS is
configured appropriately.

Do not treat claims such as "HAGS always gives +5% FPS" as universal
truth.

------------------------------------------------------------------------

## 💽 Use an SSD

STALKER 2 should be installed on an **SSD**.

An NVMe SSD is preferable when available, but the important distinction
is avoiding a mechanical hard drive for a modern streaming-heavy
open-world game.

------------------------------------------------------------------------

## 🌡️ Check Temperatures and Clock Speeds

Poor performance is not always a graphics-setting problem.

Monitor GPU/CPU temperatures, clock speeds, and GPU power utilization.

If hardware is overheating and throttling, changing Shadows from High to
Medium is treating the symptom rather than the cause.

------------------------------------------------------------------------

# Advanced Troubleshooting

## 📊 Use a Performance Overlay

Tools such as **MSI Afterburner / RTSS** or GPU-driver overlays can help
determine *why* performance is poor.

Useful metrics include FPS, 1% lows, frame time, GPU utilization, GPU
clock, VRAM usage, CPU utilization, per-core CPU utilization, system RAM
usage, and temperatures.

### A Simple Diagnostic Rule

If the GPU is sitting near **95--100% utilization**, you are probably
primarily **GPU-limited**. Lowering GPU-intensive settings or using
upscaling may help.

If GPU utilization is substantially below maximum while one or more CPU
threads are heavily loaded, you may be **CPU-limited**. Reducing
resolution will not necessarily solve a CPU bottleneck.

------------------------------------------------------------------------

## 📈 Frame Time Is Often More Useful Than FPS

FPS tells you how many frames are produced.

**Frame time tells you how consistently they arrive.**

A large spike on a frame-time graph corresponds directly to the hitch
you feel while playing.

Use it when investigating traversal stutter, periodic hitching,
shader-related stalls, asset-streaming problems, and background-process
interruptions.

------------------------------------------------------------------------

## 🧰 Process Lasso --- Advanced and Optional

Process Lasso can be useful for advanced CPU-affinity, scheduling, and
process-priority troubleshooting.

It is **not required for Borscht**, and you should not automatically
assign STALKER 2 extreme priorities because somebody on the Internet
said to.

If you use Process Lasso, make deliberate changes and test them
individually.

------------------------------------------------------------------------

## 🧹 Background Applications

Browsers with dozens of tabs, game launchers, RGB suites, recording
software, overlays, cloud-sync applications, and other background
processes consume some combination of CPU time, RAM, VRAM, GPU
resources, and storage I/O.

You do not need to turn your gaming PC into a sterile laboratory. Just
make sure something unnecessary is not consuming a meaningful portion of
the resources STALKER 2 needs.

------------------------------------------------------------------------

## 🎥 Recording and Streaming

OBS, Discord streaming, browser video, NVIDIA recording features, and
similar applications can consume GPU resources and VRAM.

If STALKER 2 performs well normally but poorly while recording or
streaming, test without those workloads before changing the game's
graphics configuration.

------------------------------------------------------------------------

## 🖥️ G-SYNC / FreeSync and Frame Caps

Variable Refresh Rate technologies such as **NVIDIA G-SYNC** and **AMD
FreeSync** can improve perceived smoothness when frame rate varies
within the monitor's supported VRR range.

A sensible frame-rate cap can also improve consistency.

> **Consistency beats screenshots of an FPS counter.**

------------------------------------------------------------------------

# Things Borscht Does NOT Recommend

## ❌ Disabling Windows Security Features for FPS

Some optimization guides recommend disabling Windows security
technologies such as **Core Isolation / Memory Integrity**.

Borscht does **not** recommend disabling operating-system security
features as a general performance tweak.

------------------------------------------------------------------------

## ❌ Blind Registry Tweaks

Do not import random `.reg` files advertised as gaming latency fixes,
network optimizers, ultimate FPS tweaks, CPU unlockers, or RAM
optimizers unless you understand exactly what they change.

A registry file being downloadable does not make it good engineering.

------------------------------------------------------------------------

## ❌ "Optimization Packs"

Avoid collections that change dozens or hundreds of undocumented
Windows, driver, Unreal Engine, or game settings simultaneously.

If performance improves, you will not know why.

If something breaks, you will not know why.

That is the opposite of troubleshooting.

------------------------------------------------------------------------

# Recommended Troubleshooting Order

If Borscht is performing poorly, work through this order before asking
for support:

1.  **Reset the in-game Graphics settings.**
2.  Select an overall preset appropriate for your hardware.
3.  Test before adding additional optional visual enhancements.
4.  Reduce **Rendering Distance** and **Shadows** if necessary.
5.  Check **VRAM usage** and reduce Texture Quality if VRAM is
    exhausted.
6.  Enable an appropriate **upscaling** quality mode if needed.
7.  Establish acceptable underlying performance.
8.  Enable **Frame Generation** if supported and desired.
9.  Add optional Borscht visual enhancements one at a time.
10. Monitor FPS, frame time, GPU utilization, VRAM, CPU usage, and
    temperatures if problems remain.
11. Only then move into advanced system-level troubleshooting.

------------------------------------------------------------------------

# Final Thoughts

There is no single magical STALKER 2 performance configuration.

Two PCs with similar-looking specifications can behave differently
because of resolution, VRAM, CPU limitations, memory configuration,
thermals, background applications, driver versions, and the visual
features being used.

The goal is not:

> **MAKE NUMBER BIG.**

The goal is:

> **Good image quality + responsive controls + consistent frame pacing +
> stable gameplay.**

Find the balance that works for **your hardware** and then go enjoy the
Zone. ☢️

------------------------------------------------------------------------

*This guide will continue to evolve as Borscht, S.T.A.L.K.E.R. 2,
graphics drivers, and supported rendering technologies are updated.*

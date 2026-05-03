# MyOS x64

MyOS x64 is a performance-focused Linux distribution built for users who want more than a default desktop image. It combines a custom kernel line, snapshot-aware installation logic, lightweight resource handling, and a bundled toolchain designed to make gaming, production, and day-to-day system management feel faster, cleaner, and more controlled.

This repository is the main project home for MyOS x64. The separate kernel and standalone tools delivery flows are published through their own GitHub repositories, which are linked below.

## Why MyOS x64

MyOS x64 is designed around a simple idea: the operating system should not force the user to stitch together performance tuning, system recovery, package setup, and low-level controls by hand after installation. Instead of shipping a bare desktop and leaving the rest to terminal work, MyOS aims to provide an opinionated, ready-to-use environment where the important system layers already work together.

The result is a distribution focused on:

- faster desktop response
- lower-latency daily use
- smoother gaming sessions
- cleaner post-install setup
- easier access to system-level controls
- stronger recovery and maintenance flow through BTRFS-aware design

## Built-In MyOS Tools

One of the strongest parts of MyOS x64 is that its system experience is not built around random third-party panels. It ships with its own toolchain, designed to expose the parts users actually change and care about.

### MyOS Control Center

MyOS Control Center is the central command panel of the distribution. Instead of jumping between terminal commands, config files, and several disconnected utilities, users get one place for practical system control.

It is built to make daily administration simpler and faster by bringing together:

- DNS profile switching
- privacy and security focused DNS options
- firewall and NetSec controls for blocking risky or unwanted IP ranges
- kernel selection and update flow
- power profile switching
- GPU tweaks and I/O Boost style performance controls

The real advantage is not only convenience. It gives MyOS a more coherent identity as a distribution that treats performance, security, and usability as parts of the same control surface.

### MyOS Scaler

MyOS Scaler is the gaming-side performance utility of the project. It is built for users who want more control over how games are launched, scaled, monitored, and tuned.

Its role is not limited to image scaling. It brings together a practical gaming stack that can help improve smoothness and visibility during gameplay:

- Gamescope-based scaling flow
- FSR and NIS support for cleaner output from lower internal resolutions
- Steam launch integration
- MangoHud metrics for FPS, frametime, temperatures, and system load
- GameMode helpers for giving the game better resource priority
- ZRAM status visibility as part of the broader performance picture

In practice, this means MyOS is not only trying to look gaming-oriented on paper. It provides actual tools to pursue more stable frame pacing, easier monitoring, and a more controlled play session.

### MyOS Package Installer

MyOS Package Installer is designed to reduce one of the most repetitive parts of a fresh Linux setup: rebuilding the software stack from scratch. Instead of forcing the user to manually hunt packages one by one, it presents applications through a more curated and category-based flow.

This helps users move faster from a clean installation to a complete working desktop by organizing software such as:

- daily tools
- media applications
- office software
- store and software hub entries
- gaming software
- system utilities

The value here is speed, clarity, and a better first-week experience after installation.

### MyOS Installer and Dual Boot Flow

MyOS Installer is built to make deployment more practical for real users, not just clean virtual machines. It can detect existing Windows and Linux installations, work with side-by-side layouts, shrink selected partitions when needed, and preserve the existing EFI structure while integrating systems into the GRUB boot flow.

That gives MyOS x64 a more realistic migration path for users who want to test or adopt the system without wiping an existing machine.

### MyOS Hello

MyOS Hello acts as the first-boot entry point. It helps connect the user to the rest of the MyOS ecosystem by surfacing shortcuts, themes, and quick access paths to the most important tools right after startup.

## Custom Kernel Advantages

MyOS x64 does not treat the kernel as an afterthought. The custom MyOS kernel line is one of the main reasons the distribution feels different in actual use.

Key advantages include:

- separate Intel and AMD optimized kernel channels
- BORE scheduler based performance direction
- built-in storage and boot-critical drivers for a cleaner startup path
- lower-latency oriented desktop behavior
- gaming-aware tuning philosophy
- better continuity between the live environment and the installed system

Rather than shipping a completely generic kernel and expecting the user to optimize later, MyOS uses the kernel layer as part of the operating system identity. That benefits boot consistency, responsiveness, and the overall feel of the system under load.

## BTRFS, Snapshots, and Recovery Mindset

MyOS x64 is not only focused on speed. It also pays attention to recoverability and maintenance. When BTRFS is used, the system is designed around a snapshot-aware layout that works with subvolumes, Snapper-style flows, and grub-btrfs visibility.

The advantage is straightforward: system changes are easier to track, rollbacks become more practical, and maintenance does not feel like a blind jump.

## Developer-Ready Foundation

MyOS x64 also targets users who build, script, test, and tinker. Alongside its gaming and desktop focus, it ships with a stronger technical base for real work.

That includes a foundation suited for:

- C and C++ development through base-devel
- Python-based workflows
- PyQt6 application work
- Go development
- disk, networking, and virtualization tasks

This makes MyOS useful not only as a performance desktop, but also as a working environment for users who actually build software and tools on the same machine.

## Related Repositories

The MyOS project is split into clear components so users can follow the part they care about most.

- Main project: [ITLABSofficial](https://itlabsofficial.github.io/)
- MyOS Kernel: [ITLABSofficial/MyOS-Kernel](https://github.com/ITLABSofficial/MyOS-Kernel)
- MyOS Tools: [ITLABSofficial/MyOS_Tools](https://github.com/ITLABSofficial/MyOS_Tools)
- Issues and support: [MyOS x64 Issues](https://github.com/ITLABSofficial/MyOs-x64/issues)

## Project Direction

MyOS x64 is built for users who want a Linux system that already ships with stronger defaults, clearer system tools, and a more performance-aware foundation. The goal is not to be the most minimal distribution. The goal is to be more usable, more controlled, and more purpose-built from the first boot onward.

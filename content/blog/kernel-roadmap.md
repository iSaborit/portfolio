+++
title = "I'm Building a Microkernel in Rust — Here's My Roadmap"
date = 2026-09-05
description = "Four chapters of a plan to get from shipped developer tools to a real microkernel: what I'm building, in what order, and why."
draft = true
[taxonomies]
tags = ["rust", "kernel", "os", "systems"]
+++

I like breaking computers to understand how they work, then building better ones. That's the whole reason I got into systems — and it's also why this site's roadmap section is about to get real.

This post is my plan, written down so I can't wimp out of it.

## The arc

"Silicon to shell": bare-metal code, kernels, devices, and the tooling that makes complex systems legible instead of intimidating. Four chapters, each feeding the next.

## Chapter 1 — a developer tool people actually use

Before anything fancy, I need something shipped. A small Rust tool that makes a low-level thing legible — think a syscall trace pretty-printer, or an ELF analyzer that explains what a binary is doing in plain language. Published on crates.io, with a launch post people actually see.

Shipped beats ambitious. A tool with ten real users says more than ten star-wars kernels nobody runs.

## Chapter 2 — the microkernel

The long arc. Following the phil-opp "Writing an OS in Rust" curriculum as a warm-up, but with a rule: don't type along, re-express each design in my own words. Then the interesting part:

1. **A fixed-priority real-time scheduler** — with priority inheritance and deadline tracking. This is where my embedded/safety-critical training (real-time systems, FreeRTOS-class scheduling) stops being theoretical.
2. **L4-style IPC with a capability model** — the microkernel flag. Two user tasks talking through kernel-mediated message passing, no shared memory.
3. **Real hardware** — a Raspberry Pi port, plus writeups of the hard parts.

## Chapter 3 — a device that bridges to tooling

Rust firmware on a real microcontroller (RP2040-ish), running a real scheduler or a comms protocol — then a companion dashboard showing what the device is doing live. The embedded part and the "make it legible" part in one project.

## Chapter 4 — one meaningful open-source contribution

Not a project, a merge. One non-trivial PR to an established project that I can talk about for half an hour.

## The honest part

Projects get you the interview; they don't pass it. So in parallel: daily algorithms and data-structures practice, and system-design fundamentals (concurrency, caching, memory). No project list replaces that.

The timeline is ~18 months, hitting milestones every few weeks, with this site's Projects and blog as the public log. First chapter ships this year — I'll post here when it does.
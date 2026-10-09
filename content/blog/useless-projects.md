+++
title = "Do What You Don't Want"
date = 2026-07-26
description = "Stuck waiting for the perfect idea, I built a deliberately useless htop clone instead — and learned more in ten hours than in months of thinking."
[taxonomies]
tags = ["learning", "systems", "rust"]
+++

*Written Jul 26, 2026 — cleaned up and reframed Oct 2026.*

I spent years waiting for the perfect idea to strike. I never thought of myself as creative, yet I was overflowing with half-ideas. Ambitious, too — so ambitious that I felt I needed to do something big. But nothing ever aligned perfectly with my goals, so I'd sit there, notebook open, pen in hand, waiting for inspiration.

Here's the embarrassing truth: I never did anything. Not big, not small. Just thinking, with the quiet certainty that someday, maybe, I would do something big.

## The freeze

The pattern was always the same. An idea would show up, and immediately the flaws would show up with it: wrong environment, wrong scope, wrong timing — or just my own self-confidence quietly vetoing it. Every idea had to survive a trial before a single line of code existed, and none of them did.

Then, last year, I hit a wall. My ambition was screaming for more, but my fear of "not big enough" kept me frozen. So I made a rule, deliberately crude: do something — anything — now. No more waiting for perfection.

## A deliberately useless project

I'm a programmer, for better and for worse, so I did what I always do to learn something: reinvent the wheel. I picked the most useless project I could think of — a kind of htop, a terminal task manager. Nobody would ever use it. Not even me.

That was exactly the point. With zero expectations, there was nothing to live up to. I opened my editor and just wrote code: processes, refresh loops, sorting, the unglamorous plumbing of reading what the OS is doing and putting it on screen.

It wasn't optimal. It wasn't even good. But it was done — and finishing it felt amazing. For the first time in ages I had something that ran, something I could point at, instead of another page of notes about something I might build.

That throwaway project grew up into [custom_top](@/projects/custom-top.md): a `top`-style process monitor written in C. Still a learning spike, never a product — but a finished one, and public on GitHub.

## What ten hours of "useless" taught me

I did a couple more of these nonsense projects, and they taught me my actual limits far better than hundreds of hours of blank-page staring ever had. Three lessons stuck:

**1. Constraints breed creativity.** I wasn't uncreative because I lacked ideas — I was uncreative because I believed I had unlimited possibilities. Blank canvases are terrifying. It was only when I forced myself to build within arbitrary, absurd constraints that my brain started finding creative solutions that actually fit me and my environment. Orson Welles said the enemy of art is the absence of limitations. My terminal task manager proved him right.

**2. Know your tools by abusing them.** Pushing my tooling to its limits showed me where those limits were, and those limits pushed me further. Writing close to the OS in C, fighting with syscalls and process tables, clarified something important: my home is at the low-level end of the spectrum. Rust and C, systems code, the layers most people never see. I didn't reason my way there — I built my way there.

**3. Done beats perfect, every time.** Ten hours on a "useless" project generated more real ideas than months of waiting for the brilliant one. Each finished thing, however small, made the next idea cheaper to try.

## The point

Not every project needs to be ambitious. Some just need to be finished. If you're stuck the way I was — notebook open, standards impossibly high, output at zero — pick the small useless thing and build it this weekend. Lower the stakes until starting is easy, then let finishing do its work.

You can see what that approach produced for me in [my projects](@/projects/_index.md). None of them started as a good idea. They started as something to do instead of nothing.

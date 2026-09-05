+++
title = "rudist"
date = 2026-09-05
description = "A Redis-compatible server you can debug against — observability-first, built for local dev and CI."
[extra]
status = "in progress"
github = "https://github.com/iSaborit/rudist"
[taxonomies]
tags = ["rust", "redis", "networking", "systems"]
+++

A Redis-compatible server whose real gift is being able to see inside: `MONITOR`/`INFO`/`SLOWLOG`, a simulated clock for deterministic tests, and a full JSON state dump. Built for the dev-loop and CI, not production.
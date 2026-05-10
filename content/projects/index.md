---
title: "Projects"
date: 2026-02-04
draft: false
---

## [Cthaeh](https://github.com/jeffaf/cthaeh)
🌳 Ghidra-powered triage scanner for Windows kernel drivers. Used as part of my driver research workflow, including findings later published as CVEs. Scores drivers on 60+ vulnerability heuristics so you know which `.sys` files to pull apart first. Named after the all-seeing tree from *The Kingkiller Chronicle*.

## Vulnerability Research

### [CVE-2026-3508: ASUS AsusWmiAcpi.sys Heap Over-Read](https://github.com/jeffaf/publications/tree/main/CVE-2026-3508)
Kernel driver research finding in ASUS System Control Interface. The issue was a `METHOD_BUFFERED` IOCTL size validation bug where the driver trusted an embedded length field and read beyond the actual buffered input allocation.

### [CVE-2026-6737: ASUS AsusPTPFilter.sys Insecure Device Object Permissions](https://github.com/jeffaf/publications/tree/main/CVE-2026-6737)
ASUS Precision Touchpad Filter driver issue where named device objects were created without explicit SDDL permissions, exposing driver IOCTL handlers to standard local users. Fixed in `AsusPTPFilter` version `16.0.0.46` or later.

## [Cred Relay](https://credrelay.com)
Monthly newsletter covering offensive security, maldev, and AI-assisted security research.

## [CVE-2025-3464 AsIO3 LPE](https://github.com/jeffaf/CVE-2025-3464-AsIO3-LPE)
BYOVD LPE exploit for ASUS AsIO3.sys - TOCTOU auth bypass + PreviousMode decrement to steal SYSTEM tokens on Windows 11. AI-assisted exploit development. CVE discovered by [Cisco Talos](https://blog.talosintelligence.com/decrement-by-one-to-rule-them-all/).

## [Bluesky CLI](https://github.com/jeffaf/bluesky-skill)
Full-featured CLI for Bluesky/AT Protocol. Post, reply, like, repost, follow, block, mute, search, threads, and images from the terminal.

## [NimSysLoader](https://github.com/jeffaf/NimSysLoader)
A Nim-based shellcode loader that utilizes direct syscalls via NimlineWhispers2/SysWhispers2 for core functionality.

## [Bazzy](https://github.com/jeffaf/bazzy)
A shellcode injector and runner built in Nim.

## [BunnyGod](https://github.com/jeffaf/bunnygod)
AI-powered philosophical Q&A system that retrieves answers from academic literature. Built with Astro, Cloudflare Workers, and Workers AI.

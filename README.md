---
title: SoundDash
description: Route Mac system audio to multiple outputs with per-output channel mapping, shared volume, and sound controls.
platform: macOS
language: Swift
---

# SoundDash

SoundDash is a native macOS menu-bar app for routing your Mac’s system audio to one or more selected audio outputs at the same time. Choose Left, Stereo, or Right channel mode for each output:

```text
Left    L/L   The source’s left channel plays through both output channels.
Stereo  L/R   The original left and right channels stay in stereo.
Right   R/R   The source’s right channel plays through both output channels.
```

## Features

- Add, remove, and configure output routes.
- Identify connected devices with a test tone; distinguish devices with aliases.
- Control shared volume and mute, plus individual output levels and mute.
- Adjust stereo balance and a 10-band equalizer.
- Start or stop routing from the dashboard or menu-bar popover.
- Save output assignments and sound settings on your Mac.

SoundDash uses Core Audio device IDs to keep assignments tied to devices. It captures system audio for real-time routing and does not record or save audio.

## Built with

Swift, SwiftUI, and Apple Core Audio. The Xcode project’s macOS deployment target is 14.6.

## Scope

SoundDash currently supports Left, Stereo, and Right channel modes. AirPlay routing, recording, per-app mixing, and arbitrary routing graphs are outside the current scope. Synchronization behavior may vary across output hardware.

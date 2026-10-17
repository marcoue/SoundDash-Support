---
title: SoundDash
description: Route Mac system audio to multiple audio outputs with per-output channel mapping, sound controls, profiles, and AirPlay support.
platform: macOS
language: Swift
---

# SoundDash

[SoundDash](https://dashapps.app/sounddash/) is a native macOS menu-bar app for routing your Mac’s system audio to multiple selected audio outputs. Configure a channel mode for each output:

```text
Left           L/L   The source’s left channel plays through both output channels.
Stereo         L/R   The original left and right channels stay in stereo.
Reverse Stereo R/L   The source’s right and left channels are swapped.
Right          R/R   The source’s right channel plays through both output channels.
```

## Features

- Add, remove, and configure output routes.
- Route audio to connected Core Audio devices and supported AirPlay receivers.
- Identify devices with a test tone and distinguish them with aliases.
- Control master volume and mute, plus individual output levels, mute, and stereo balance.
- Adjust a 10-band equalizer, use built-in sound presets, and save custom EQ presets.
- Create named profiles for routing and sound settings.
- Adjust AirPlay output timing with synchronization test controls. Results may vary by receiver and network.
- Start or stop routing from the dashboard or menu-bar popover.
- Save settings locally, or export and import them with device remapping when moving between Macs.

SoundDash uses persistent device identifiers to keep saved assignments associated with their outputs. Captured system audio stays in memory for real-time routing; SoundDash does not record or save audio.

## Built with

Swift, SwiftUI, and Apple Core Audio. The Xcode project’s macOS deployment target is 14.6.

## Scope

SoundDash supports the four channel modes listed above. AirPlay receiver compatibility and synchronization can vary. Recording, per-app mixing, and arbitrary routing graphs are outside the current scope.

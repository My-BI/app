# System requirements — macOS

*Current as of MyBI 26.1.0, 11 August 2026.*

## The short version

**macOS 12 Monterey or later, on any Mac from roughly 2015 onwards.** Apple Silicon and Intel both run
natively — MyBI ships as a universal app, so there is one download and no wrong choice.

## Supported Macs

Every Mac that can run macOS 12 Monterey, which is the oldest release MyBI supports:

| Model | Supported from |
|---|---|
| MacBook Air | Early 2015 and later |
| MacBook Pro | Early 2015 and later |
| MacBook | Early 2016 and later |
| iMac | Late 2015 and later |
| Mac mini | Late 2014 and later |
| Mac Pro | Late 2013 and later |
| iMac Pro | 2017 (all models) |
| Mac Studio | 2022 and later |
| Any Apple Silicon Mac | M1 and later |

If your Mac is running Monterey or newer, it can run MyBI. Apple's own Monterey compatibility list is
the authority on which machines reach that version.

## Hardware

| | Minimum | Comfortable |
|---|---|---|
| Memory | 4 GB | 8 GB or more |
| Disk | 1 GB free | 5 GB or more with several projects open |

Datasets are held and queried on your own machine, so memory is what decides how large a dataset
stays comfortable rather than any licence tier.

## What needs a newer macOS, or Apple Silicon

Everything below is additional. MyBI's core — importing data, building dashboards, charts, the
canvas, projects, publishing, encryption, sign-in — works on every supported configuration. A
feature your Mac cannot run is simply not shown, rather than shown and refused.

| Feature | Needs |
|---|---|
| On-device Whisper transcription | macOS 13 |
| MLX local AI models | macOS 14, Apple Silicon |
| In-app purchase | macOS 15 |
| Apple Intelligence | macOS 26, Apple Silicon |
| Age verification via the system | macOS 26 |
| On-device embedding — semantic search, retrieval, AI data chat | Apple Silicon |

The last row is the one that catches people out: it is an **architecture** limit rather than an OS
one, because the runtime those models need publishes no Intel-Mac build. An Intel Mac can still use
the assistant with your own cloud API key.

## Also worth knowing

- An internet connection is needed to sign in, to publish, to fetch language packs and colour
  palettes, and to check for updates. Building dashboards from your own files needs none.
- MyBI is distributed through the Mac App Store.

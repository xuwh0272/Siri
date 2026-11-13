# Siri + Dynamic Island for Windows

Latest public source snapshot: **2026-11-13**.

This repository contains the current Windows source for:

- **SiriAI** — the WPF Siri experience, animated glass orb, answer panel, local-model routing, live background capture, and Liquid Glass refraction.
- **DynamicIsland** — the Windows Dynamic Island shell, media, network, timer, clipboard, AirDrop-style transfer, usage card, and the direct Siri handoff animation.

## Highlights in this snapshot

- Direct Dynamic Island-to-Siri shared animation instead of an overlay/cross-fade.
- iOS-style Liquid Glass background refraction and RGB dispersion.
- `LiquidGlassWpf.cs` optical model and a DirectX 12 compute path that can select an NVIDIA GPU.
- CPU fallback when the DirectX 12 device is unavailable.
- Updated Siri question/answer UI and Dynamic Island usage display.

## Requirements

- Windows 10/11
- .NET 8 SDK for the Dynamic Island and capture helper
- A separately configured local model/runtime if you want local AI replies

The model files, API keys, private configuration, logs, conversations, caches, backups, and compiled output are intentionally not included.

## Build

```powershell
dotnet build .\DynamicIsland\DynamicIsland.csproj -c Release
dotnet build .\SiriAI\src\LiquidGlassCapture\LiquidGlassCapture.csproj -c Release
```

`SiriAssistant.cs` is the current Siri application source. The local-model executable and model path must be configured for your own machine.

## Source layout

```text
DynamicIsland/       Windows Dynamic Island WPF source and assets
SiriAI/src/          Siri application and Liquid Glass source
NOTICE.md            attribution and third-party notice
```

## Project notice

This is an independent Windows project and is not affiliated with Apple, OpenAI, Anthropic, Google, or Microsoft. Third-party names and marks belong to their respective owners.

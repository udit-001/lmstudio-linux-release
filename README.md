<h1 align="center">
  <img align="top" width="44" src="https://raw.githubusercontent.com/udit-001/lmstudio-linux-release/refs/heads/main/assets/logo44.png">
  <span>LM Studio Linux Releases</span>
</h1>


<p align="center">
  <a href="https://github.com/udit-001/lmstudio-linux-release/releases/latest" target="_blank"><img alt="release" src="https://img.shields.io/github/v/release/udit-001/lmstudio-linux-release?label=release&labelColor=%231e1e2e&color=%2300D4AA"></a>
  <span> </span>
  <a href="https://github.com/udit-001/lmstudio-linux-release/actions/workflows/release.yml" target="_blank"><img alt="downloads" src="https://img.shields.io/github/actions/workflow/status/udit-001/lmstudio-linux-release/release.yml?branch=main&labelColor=%231e1e2e&color=%2300D4AA"></a>
  <span> </span>
</p>

## Overview

GitHub Action to fetch the latest **LM Studio** Linux builds (AppImage & DEB) and create a release.

## Why?

LM Studio on Linux:
- ❌ Doesn't auto-update
- ❌ Doesn't provide a fixed versioned download URL
- ✅ Has direct download links for latest builds

This makes it hard for Linux users to keep LM Studio up to date & this action solves that by:
- Fetching the latest version from LM Studio's download redirects
- Checking if that version already exists as a GitHub release
- If not, downloading all formats (AppImage & DEB for x64 and arm64) and publishing a release

Linux users can then update via GitHub releases, scripts, or package managers using a consistent URL.

## Available Downloads

Each release includes:
- **x64 (AMD/Intel)**: AppImage & DEB
- **ARM64**: AppImage & DEB

## Setup Auto Updates with Gear Lever

To automate updates for your LM Studio AppImage on Linux, use [Gear Lever](https://github.com/mijorus/gearlever). It supports update sources like GitHub releases and static URLs. Configure the update URL based on your system architecture:

- **x86_64 (AppImage)**
  ```
  https://github.com/udit-001/lmstudio-linux-release/releases/download/*/LM-Studio-*-x64.AppImage
  ```

- **ARM64 (AppImage)**
  ```
  https://github.com/udit-001/lmstudio-linux-release/releases/download/*/LM-Studio-*-arm64.AppImage
  ```


These URLs will allow automatic fetching of the latest releases. For more detailed instructions, refer to the [update guide](https://mijorus.it/posts/gearlever/update-url-info/).

## 📅 Release Status
- **⏳ Last Released On**: 2026-02-14 14:46:57 UTC
- **🔄 Last Run**: 2026-02-18 02:23:23 UTC

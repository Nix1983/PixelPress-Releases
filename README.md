# Pixel Press

[![Website][badge-website]][product-page]
[![Windows Store][badge-windows-store]][windows-store]
[![Debian release][badge-debian-release]][latest-release]
[![User Wiki][badge-user-wiki]][wiki]
[![License](https://img.shields.io/badge/license-proprietary-6f42c1)](#license)

Pixel Press is a local desktop image optimizer for turning JPEG, PNG, WebP, and
AVIF files into smaller WebP or AVIF output. Your images stay on your machine,
there are no uploads, and original files stay untouched.

Perfect for website images, screenshots, product folders, and quick batch
optimization before publishing.

This repository is the public release home for Pixel Press. It contains Linux
release downloads, release notes, issue forms, and user documentation. The
application source code is private.

## Download

| Platform | Download |
|:--|:--|
| Windows | [Install from Microsoft Store][windows-store] |
| Ubuntu / Debian Linux | [Download the latest `.deb` package][debian-deb] |
| Product page | [ghostlyinc.com/en-us/tools/pixel-press][product-page] |

## Documentation

The full user guide is available in the [Pixel Press Wiki][wiki].

Good starting points:

- [Getting Started][wiki-getting-started]
- [Installation and Updates][wiki-installation]
- [Converting Images][wiki-converting]
- [Supported Formats and Quality][wiki-formats]
- [Output Files and Folders][wiki-output]
- [Windows and Linux Differences][wiki-platforms]
- [Pixel Press Pro][wiki-pro]
- [Troubleshooting][wiki-troubleshooting]

## Bugs and Feature Requests

Use GitHub Issues to report bugs or request user-facing improvements:

- [Report a bug][new-bug]
- [Request a feature][new-feature]

Please do not upload private photos, customer files, license information,
passwords, or other secrets in public issues.

## What It Does

- Batch-compress local images without sending them anywhere.
- Add individual files or whole folders.
- Convert supported source images to modern web-friendly formats.
- Choose WebP and/or AVIF output.
- Keep unsupported or broken files out of the conversion instead of crashing.
- Save optimized files into a separate output folder.
- Preserve folder structure for folder-based runs.
- Show size savings, output file counts, and conversion duration after a run.

## Supported Formats

| Direction | Formats |
|:--|:--|
| Input | JPEG, JPG, PNG, WebP, AVIF |
| Output | WebP, AVIF |

Available formats can depend on the bundled ImageMagick runtime used by the
build. The app only enables output formats that are supported by the current
runtime.

## Ubuntu / Debian Install

Download the latest package:

```bash
wget -O /tmp/PixelPress-linux-x64.deb https://github.com/Nix1983/PixelPress-Releases/releases/latest/download/PixelPress-linux-x64.deb
```

Install it with dependencies:

```bash
sudo apt install /tmp/PixelPress-linux-x64.deb
```

Start Pixel Press from your application launcher, or run:

```bash
pixelpress
```

## Update

Download the newest `.deb` package from the latest release and install it over
the existing version:

```bash
wget -O /tmp/PixelPress-linux-x64.deb https://github.com/Nix1983/PixelPress-Releases/releases/latest/download/PixelPress-linux-x64.deb
sudo apt install /tmp/PixelPress-linux-x64.deb
```

## Uninstall

```bash
sudo apt remove pixelpress
```

## What Pixel Press Expects

Pixel Press is designed for local image optimization jobs where you want a fresh
optimized copy and the original files left untouched.

The most reliable inputs are:

- JPEG and PNG images from cameras, websites, design exports, and screenshots.
- Existing WebP or AVIF images that you want to recompress or convert.
- Folders that contain supported images directly or in subfolders.
- Images that ImageMagick can read on the current runtime.

Pixel Press ignores unsupported, unreadable, or broken files instead of treating
them as a failed conversion for the whole batch.

## Platform Notes

Windows users should install Pixel Press from the Microsoft Store. The Store
also handles Pixel Press Pro purchases and updates.

Ubuntu/Debian users can install the `.deb` package from this repository. The
Linux release currently has its own release behavior and does not use Microsoft
Store purchases.

On Windows, drag and drop is supported. On Linux, use the file and folder picker
buttons from inside the app.

## License

Pixel Press is proprietary software by Ghostly Inc. This release repository is
not an open-source source-code repository, and no open-source license is granted
for the application source or binaries unless a separate license agreement says
otherwise.

[badge-website]: https://img.shields.io/badge/website-ghostlyinc.com-0969da
[badge-windows-store]: https://img.shields.io/badge/Windows-Microsoft%20Store-0078d4
[badge-debian-release]: https://img.shields.io/github/v/release/Nix1983/PixelPress-Releases?label=Debian%20release&logo=debian&logoColor=white&color=e95420
[badge-user-wiki]: https://img.shields.io/badge/docs-user%20wiki-2ea44f
[product-page]: https://ghostlyinc.com/en-us/tools/pixel-press/
[windows-store]: https://apps.microsoft.com/detail/9NRMXB13BBN7
[debian-deb]: https://github.com/Nix1983/PixelPress-Releases/releases/latest/download/PixelPress-linux-x64.deb
[latest-release]: https://github.com/Nix1983/PixelPress-Releases/releases/latest
[wiki]: https://github.com/Nix1983/PixelPress-Releases/wiki/Home
[wiki-getting-started]: https://github.com/Nix1983/PixelPress-Releases/wiki/Getting-Started
[wiki-installation]: https://github.com/Nix1983/PixelPress-Releases/wiki/Installation-and-Updates
[wiki-converting]: https://github.com/Nix1983/PixelPress-Releases/wiki/Converting-Images
[wiki-formats]: https://github.com/Nix1983/PixelPress-Releases/wiki/Supported-Formats-and-Quality
[wiki-output]: https://github.com/Nix1983/PixelPress-Releases/wiki/Output-Files-and-Folders
[wiki-platforms]: https://github.com/Nix1983/PixelPress-Releases/wiki/Windows-and-Linux
[wiki-pro]: https://github.com/Nix1983/PixelPress-Releases/wiki/Pixel-Press-Pro
[wiki-troubleshooting]: https://github.com/Nix1983/PixelPress-Releases/wiki/Troubleshooting
[new-bug]: https://github.com/Nix1983/PixelPress-Releases/issues/new?template=bug_report.yml
[new-feature]: https://github.com/Nix1983/PixelPress-Releases/issues/new?template=feature_request.yml

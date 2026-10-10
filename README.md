# tame-gg Scoop bucket

[![Tests](https://github.com/tame-gg/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/tame-gg/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/tame-gg/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/tame-gg/scoop-bucket/actions/workflows/excavator.yml)

[Scoop](https://scoop.sh) manifests for [Flavor](https://github.com/tame-gg/Flavor), which keeps several Tailscale and Headscale networks connected at once on Windows 11, x64 and ARM64.

```pwsh
scoop bucket add tame-gg https://github.com/tame-gg/scoop-bucket
scoop install tame-gg/flavor
```

Start the daemon with `flavord`, then open Flavor from the Start menu. Scoop doesn't start `flavord` at sign-in; the installer from the [Flavor releases](https://github.com/tame-gg/Flavor/releases) does. Stop `flavord` with `Stop-Process -Name flavord` before `scoop update flavor` or `scoop uninstall flavor`.

The manifest follows every Flavor release, prereleases included, through the Excavator workflow. Report problems in [Flavor's issues](https://github.com/tame-gg/Flavor/issues).

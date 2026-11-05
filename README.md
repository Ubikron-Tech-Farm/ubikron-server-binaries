# Ubikron private server installers

The installers for the Ubikron private server are attached to this repo's [releases](https://github.com/Ubikron-Tech-Farm/ubikron-server-binaries/releases), one file per platform:

| Platform | File |
|---|---|
| Windows | `ubikron-pro-server.exe` |
| macOS | `ubikron-pro-server-macos` |
| macOS, installs offline | `ubikron-pro-server-macos.pkg` |
| Linux | `ubikron-pro-server-linux` |
| Linux ARM64 | `ubikron-pro-server-linux-arm64` |

How to install, configure and run the server: https://ubikron.com/servers/install

## Shipping a new version

The download buttons on ubikron.com link to the latest release, for example
`https://github.com/Ubikron-Tech-Farm/ubikron-server-binaries/releases/latest/download/ubikron-pro-server-linux`.
So to ship, publish a new release with all five files, named exactly as above:

```
gh release create v1.0 ubikron-pro-server.exe ubikron-pro-server-macos ubikron-pro-server-macos.pkg ubikron-pro-server-linux ubikron-pro-server-linux-arm64 --title "v1.0" --notes "What changed"
```

Attach all five every time: a file missing from the latest release breaks its download button.

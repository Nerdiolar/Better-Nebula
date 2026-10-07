# Better Nebula

An unofficial community project with modified Nebula clients and a Windows
test build. The current beta release provides an Android APK and a standalone
Windows client.

> **Disclaimer:** This is not an official Nebula Technologies product and is
> not affiliated with or endorsed by Nebula Technologies. Use it at your own
> risk. Nebula and related names are trademarks of their respective owners.

## Current Release

**Beta 1.5.4** — [View the release and all assets](https://github.com/Nerdiolar/Better-Nebula/releases/tag/1.5.4)

| Platform | Download | Description |
|---|---|---|
| Android | [Better-nebula-v1.5.4.apk](https://github.com/Nerdiolar/Better-Nebula/releases/download/1.5.4/Better-nebula-v1.5.4.apk) | Modified Android client |
| Windows | [Better-Nebula-PC-Test-Setup.exe](https://github.com/Nerdiolar/Better-Nebula/releases/download/1.5.4/Better-Nebula-PC-Test-Setup.exe) | Complete separate client |

Download only from the repository's **Releases** page. Do not download or
install files from unverified mirrors.

## What's New in 1.5.4

- Automatically detects a connected controller and hides on-screen touch
  controls when a controller is connected.
- Adds an option to disable mouse control through touchscreen input.
- Improves Android TV support.
- Adds resolution options up to 2K and 4K, and refresh-rate options up to
  120 FPS.
- Includes adjustments intended to reduce freezes and unexpected streaming
  interruptions.
- Includes general compatibility and stability improvements.

Actual resolution, frame rate, latency, and stability depend on the device,
display, decoder, network, game, and streaming server. Selecting 4K or 120 FPS
does not guarantee the server can deliver that mode.

## Android Installation

1. Download `Better-nebula-v1.5.4.apk` from the
   [1.5.4 release assets](https://github.com/Nerdiolar/Better-Nebula/releases/tag/1.5.4).
2. Open the APK on your Android device.
3. If prompted, allow your browser or file manager to install apps from that
   source.
4. Review the Android installation prompt and continue only if you trust the
   file.

The modified APK is not an official Play Store update and may have a different
signature or application identity from the official app. Android may therefore
refuse to install it over an existing copy. Check that you can sign in again
before removing an existing app.

## Windows Installation

1. Download `Better-Nebula-PC-Test-Setup.exe` from the
   [1.5.4 release assets](https://github.com/Nerdiolar/Better-Nebula/releases/tag/1.5.4).
2. Run the installer and choose an installation folder.
3. Open **Start Menu → Better Nebula - Test Direct → Open Better Nebula (No Selector)**.
4. Sign in if requested.

This installer contains the complete test client, installs it in a separate
folder, and does **not** replace the existing Nebula installation. It launches
the client directly without the resolution selector.

The test client can share the Nebula settings and login already stored on the
same Windows account. Those personal settings and credentials are not included
in the installer.

To remove the test copy, use **Start Menu → Better Nebula - Test Direct →
Uninstall** or remove **Better Nebula - Test Direct** from Windows Installed
apps. The uninstaller removes the separate test installation, not the original
Nebula client.

> The community Windows installer is not digitally signed. Windows SmartScreen
> may show a warning. Verify that you downloaded it from the release linked
> above; do not disable security software or add broad antivirus exclusions.

## Resolution and Frame Rate

The client provides options up to 2K/1440p, 4K/2160p, and 120 FPS where
supported. To use a high-resolution or high-frame-rate mode, the streaming
server, game, client device, video decoder, display, and network all need to
support it.

If the stream stutters, try a lower mode such as 1080p at 60 FPS and check
whether the network connection is stable. Higher settings may increase
bandwidth use and decoding load.

## Troubleshooting

### Streaming or RTSP handshake errors

A successful network-port test does not necessarily mean the streaming session
has completed its RTSP negotiation. The problem may be in the client, network,
or streaming server. Restart the client and try again; if the issue continues,
contact the Nebula service provider with the error and the approximate time of
the attempt.

Do not open router ports automatically. For cloud streaming, required ports
and routing are generally controlled by the service infrastructure; port
forwarding on the client router may not help.

### Touch controls or controller detection

Reconnect the controller and restart the streaming session. If using a
Bluetooth controller, check that Android reports it as connected before
launching the stream. Touch and mouse-control behavior may differ by device.

### Windows installer or launch problems

Close any running Better Nebula test client before updating or uninstalling.
If Windows reports a missing file, download the installer again from the
official repository Release page.

## Privacy and Safe Bug Reports

- The release installer does not contain your personal Nebula profile or
  account credentials.
- The Windows test client may use the existing local Nebula profile, so its
  settings and sign-in state can be shared with the original installation.
  keys, or unreviewed logs. They may contain credentials or other private
  information.
- When reporting a problem, include the release version, device/OS, selected
  resolution and FPS, and the exact error text. Redact personal information
  from screenshots and logs first.

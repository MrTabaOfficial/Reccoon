# Security

## Reporting a problem

If you find a security problem in Reccoon, please report it privately so it can be fixed before
others learn about it:

1. Open the [Security tab](https://github.com/MrTabaOfficial/Reccoon/security) of this page.
2. Click **Report a vulnerability** and describe what you found, how to reproduce it, and which
   version you used (About page in Reccoon).

Please don't open a public issue for security problems. You'll get an answer there, usually within
a week, and credit in the release notes if you'd like it.

Ordinary bugs (crashes, wrong sound, a black recording) are welcome as normal
[issues](https://github.com/MrTabaOfficial/Reccoon/issues).

## Supported versions

Only the newest release gets security fixes. Please update before reporting.

## Getting Reccoon safely

- Download Reccoon only from this page's [Releases](https://github.com/MrTabaOfficial/Reccoon/releases).
  Copies offered anywhere else aren't official and may be changed.
- Each release lists the SHA-256 checksum of every file in `SHA256SUMS.txt`. To check a download,
  run this in PowerShell and compare the result:

  ```
  Get-FileHash .\Reccoon-x.y.z-setup.exe
  ```

- Reccoon isn't code-signed yet, so Windows SmartScreen may warn about it. That's expected for the
  files from the Releases page; for files from anywhere else, it's a reason to stop.

## What Reccoon does on your PC

- It never connects to the internet. It has no updater, no accounts, no telemetry and no ads.
- It never injects into or reads from other programs or games. It records the screen with Windows'
  own capture API and reads keys only for its shortcuts and push-to-talk.
- It installs for your user only and needs no administrator rights.

More in [PRIVACY.md](PRIVACY.md).

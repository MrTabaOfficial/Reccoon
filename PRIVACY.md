# Privacy

Reccoon collects nothing about you.

- **The internet only while you're live, or when you ask for an update.** Reccoon connects to the
  streaming server you chose (YouTube, Twitch, TikTok, or the one you typed in), only from
  *Go live* until the stream ends, and sends it your stream and your stream key, nothing else.
  When you press *Check for updates* on About, it asks GitHub for the newest version (sending only
  Reccoon's version number), and *Download and install* downloads that version from this page's
  releases. It never checks by itself. Otherwise it never connects: no accounts, no telemetry, no
  crash reports, no ads. The *GitHub page* and *Report a problem* buttons only open this page in
  your browser.
- **Stream keys** are kept in Windows Credential Manager, protected by your Windows account. They're
  never written to the settings file or the logs.
- **Your recordings stay on your PC**, in the folder you choose (`Videos\Reccoon` at first).
  Reccoon never uploads them. *Copy* puts a file on your clipboard so you can paste it yourself.
- **Settings and logs stay on your PC:** settings in `%APPDATA%\Reccoon\settings.json`, logs in
  `%LOCALAPPDATA%\Reccoon\logs`. Logs hold technical details (your graphics card, monitor and
  sound device names, the title of a window you record, errors) to help find problems. They're never sent anywhere; if you report a problem you
  can choose to attach them.
- **Keys:** Reccoon listens only for its own shortcuts and push-to-talk keys. It doesn't log or
  store what you type.
- **Microphone and sound:** recorded only while you record, stream or keep an instant replay, and
  only from the devices you chose. The level meters show sound live and keep nothing.
- **Camera (Studio):** on only while a scene shows it, in the editor's picture or in what you
  record or stream. Windows shows that the camera is in use. Nothing from it is kept except in
  your recordings, and it goes nowhere except your stream.
- **The editor (Studio)** shows the screens in your scene live while it's open, and keeps nothing.
  To list your games it reads the list of games Windows' Game Bar knows on your PC; nothing is sent.
- **Reccoon's own windows** are kept out of every capture while you record or are live, so your
  recordings and your stream never show them (or your stream key), unless you turn that off in
  Settings → Saving.
- **Instant replay** keeps the last moments in memory or in hidden temporary files that delete
  themselves; nothing is saved unless you press the replay shortcut.

Uninstalling removes the programs. Your recordings and settings stay until you delete them.

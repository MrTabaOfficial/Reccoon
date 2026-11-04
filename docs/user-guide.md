# Reccoon user guide

Everything Reccoon does, in the order you'll meet it. For a quick overview, see the
[README](../README.md).

- [Install and first start](#install-and-first-start)
- [Classic or Studio](#classic-or-studio)
- [Recording (Classic)](#recording-classic)
- [The editor (Studio)](#the-editor-studio)
- [Instant replay](#instant-replay)
- [Sound and microphone](#sound-and-microphone)
- [Live streaming](#live-streaming)
- [Your videos: Captures, trim and compress](#your-videos-captures-trim-and-compress)
- [Settings](#settings)
- [Shortcuts](#shortcuts)
- [When something doesn't work](#when-something-doesnt-work)

## Install and first start

1. Download the newest **Reccoon-x.y.z-setup.exe** from the Releases page and run it. It installs for
   your Windows user only, so no administrator rights are needed. You can also tick *Start with
   Windows*. Prefer no installer? Unzip **Reccoon-x.y.z-portable.zip** anywhere and run
   `reccoon.exe`.
2. Reccoon isn't code-signed yet, so Windows may show *"Windows protected your PC"*. Click
   **More info**, then **Run anyway**.
3. On first start, a 10-second test finds the best quality your PC can record without slowing
   games down.

Closing the window doesn't quit Reccoon. It keeps running in the tray (the raccoon icon next to
the clock), where it uses no CPU and well under 1 MB of memory. Click the tray icon to open the
window, and right-click it for a menu (record, go live, trim a video, quit).

Updating: run the new setup over the old one. Your settings and recordings stay.

## Classic or Studio

Reccoon is two apps in one. Switch any time in **Settings → About → Version**.

- **Classic** is a simple recorder. One button records your whole screen, a region you draw or
  one window. **Go live** streams the same picture.
- **Studio** is a scene editor, like OBS or Streamlabs. You place monitors, windows, games,
  pictures and text where you want them, in as many scenes as you like. **The scene you're on is
  what gets recorded, replayed and streamed**, and you can switch scenes or move things while
  you're recording or live.

New installs, and updates from Reccoon 1.0, start in Classic.

## Recording (Classic)

**Home** shows the big **Start recording** button and a summary of what gets recorded. Click a
line of the summary to change it.

- **Start / stop:** the button, or **Alt+F9** from anywhere, also inside games.
- **Pause:** **Alt+F7**, or *Pause* on Home. The video plays as if the pause never happened.
- **Marker:** **Alt+F8** marks a moment. Markers become chapters in the video, so you can jump
  to them in most players and editors.

What to record is on the **Video** page:

- **Full screen:** a whole monitor. With several monitors, pick which.
- **Region:** press **Draw region…** and drag a rectangle on the screen.
- **Window:** one program's window, even when other windows cover it.

Recordings are saved in `Videos\Reccoon` (change it in **Settings → Saving**), named like
`Reccoon 2026-11-04 21-14-03.mp4`. If the PC freezes or loses power while recording, everything
up to that moment still plays.

## The editor (Studio)

In Studio, the editor is your home: the picture at the top, and **Scenes**, **Items** and
**Mixer** below it. The bar at the bottom has **REC**, **Save replay**, your stream's
platform and quality, and **Go live**.

### Scenes

- **+** adds a scene. Click a scene to show it (also while recording or live).
- Click the pencil on the shown scene to rename it. Right-click a scene for **Rename**,
  **Duplicate** and **Delete**.
- Drag a scene up or down to reorder the list.

### Items

**+** in Items adds:

- **Screen…:** a whole monitor (**Full screen**) or one program (**Window**).
- **Game capture…:** a game. The list shows only games: the ones Windows recognises as games on
  your PC, and games from Steam, Epic, Xbox, Riot, GOG, Ubisoft, EA, Rockstar or Battle.net
  folders. If the game isn't running yet, add it anyway: it stays black until you start the
  game, and it's found again every time you restart the game.
- **Picture…:** a PNG or JPG, for example a logo or a frame.
- **Text:** a line of text, for example your Discord or a sponsor.

A Screen or Game capture opens its settings straight away. Choose what it shows, then press
**Add** (or **Cancel** to add nothing).

On the picture:

- **Drag** an item to move it; it snaps to the edges.
- **Drag the small square** in its corner to resize it.
- **Right-click** an item, either on the picture or in the Items list, for **Edit…**,
  **Hide/Show**, **Lock/Unlock**, **Bring forward**, **Send back** and **Remove**.
- **Double-click** an item to edit it.
- **Drag** items up or down in the Items list to change what's on top.

Screens and windows always keep their own shape, so nothing is stretched. If you resize a
captured window, its item follows. Windows show only what the program draws, without an empty
title bar.

### The Edit window

Each item has its own window with everything about it:

- **Screens:** **Full screen** (choose a monitor) or **Window** (choose a program). ↻ updates
  the list after you open something new.
- **Games:** the list of running games.
- **Pictures:** **Change…** picks another file.
- **Text:** the text, a colour (five swatches or any `#RRGGBB`), and a dark outline that keeps
  it readable on any background. The text is as tall as its box.
- **Position and size** in pixels of the final picture, **Fill the picture** and **Center**.
- **Shown** and **Locked**.

Every change shows at once, in the editor and in a recording or stream that's running.

### The live picture

The editor shows your screens live, up to 60 frames a second, exactly as they're recorded. It
only runs while the editor is open; minimized or in the tray it costs nothing.

While you record or are live, Reccoon keeps its own windows out of the picture, so your stream
never shows Reccoon or your stream key. The rest of the time, the editor shows Reccoon's own
window as a dark box (instead of a picture inside a picture inside a picture). You can turn the
hiding off in **Settings → Saving**.

### The mixer

Each sound device and microphone has a level meter and a volume slider. When you record only
certain apps, the mixer shows those apps instead of the devices. Change volumes before
you start: while recording or live, the sliders are locked (changes apply to the next
recording). If a microphone sends only silence, the mixer says *"Silent: muted on the
headset?"*, because a muted headset is the usual reason.

## Instant replay

Turn on **Settings → Replay → Keep the last moments ready to save**. Reccoon then keeps the last
30 seconds to 5 minutes (you choose), and **Alt+F10** (or *Save instant replay*) saves them as a
video. It works while you record too.

The moments are kept in memory, or on disk if your PC is short of RAM (**Where the last
moments are kept → Disk**). Nothing is saved unless you press the shortcut.

## Sound and microphone

**Settings → Sound** records the sound of your PC.

- **Sound devices:** everything you hear on these devices, for example HyperX *Game* and *Chat*
  together. Each has a volume.
- **Only certain apps:** only the programs you add, for example the game and Discord but not
  Spotify. An app shows up in the list while it's playing sound. Each app has its own volume.

For each source you choose:

- **Heard in the video:** part of the sound everyone hears.
- **Heard + editing track:** also as its own track in the file, so a video editor (DaVinci
  Resolve, Premiere, CapCut) can turn it down later.
- **Editing track only:** only as its own track, not in the sound people hear.

**Settings → Microphone** has up to two microphones:

- **Push-to-talk:** your voice is recorded only while one of your keys or mouse buttons is held
  (*Hold*), or switched on and off with a press (*Toggle*). The keys still work in your game.
  Reccoon keeps a moment before the press and after the release, so no word is cut off.
- **Reduce background noise:** removes fans and keyboard clicks.
- **Mute the microphone when it's quiet:** silence between words stays silent.

## Live streaming

### Setting it up

Open **Settings → Stream** (in Classic, **Stream** in the menu or **Settings** next to Go live on
Home). Choose where to stream:

- **YouTube:** YouTube Studio → *Create* → *Go live* → *Stream* → copy the *Stream key*. Try it
  first with a *Private* stream.
- **Twitch:** dashboard.twitch.tv → *Settings* → *Stream* → *Primary stream key*.
- **TikTok:** TikTok LIVE Producer → stream with a streaming software. Paste both the *Server*
  and the *Stream key*: TikTok gives you new ones each time.
- **Custom:** any other service (Kick, Facebook, your own server): paste the server address
  (`rtmp://…` or `rtmps://…`) and the key.

Your stream key is kept in Windows Credential Manager, protected by your Windows account. It's
never written to Reccoon's settings or logs, and **Show** reveals it only while you look.

**Quality:** 720p, 1080p, 1440p (YouTube encodes 1440p streams much sharper, even for 1080p
viewers) or 4K, and the bitrate. Each platform starts with what suits it, for example YouTube
1440p at 18 Mbps and Twitch about 6 Mbps. Your upload should be about one and a half times the
bitrate.

### Going live

Press **Go live** in the editor's bar or on Classic's Home, or use the tray menu. Classic streams
your screen; Studio streams the scene you're on. You can record at the same time; the
recording keeps its own quality.

On a weak connection Reccoon lowers the bitrate by itself instead of freezing. If the connection
drops, it reconnects by itself, for up to two minutes. **End stream** stops it.

Reccoon connects to the internet only while you're live, and only to the server you chose.

## Your videos: Captures, trim and compress

**Captures** lists every video Reccoon saved, by month, with a picture of each. Click the
picture to play it. The buttons:

- **Trim or compress** opens the trim window.
- **Show in folder** opens it in Explorer.
- **Delete** moves it to the Recycle Bin.

**Trim or compress** (also on Home next to the last saved video, and in the tray menu):

- **Part to keep:** drag the two handles, or type Start and End times.
- **Save trimmed copy:** keeps that part instantly, at full quality, with every sound track.
- **Compress for Discord:** makes the part fit 10 MB, 50 MB or 500 MB (Discord's limits), or a
  size you type. Then **Copy** and paste it straight into Discord with Ctrl+V.

## Settings

- **Video:** resolution and FPS (up to what your monitor shows), and *Test this PC* to find the
  best quality again. Options marked **⚡ strong PC** (4K, 120 fps) are for strong PCs, and
  Reccoon warns you if the test found them too much for yours. **Advanced** has:
  - the codec (HEVC, H.264 or AV1);
  - frame timing (skip unchanged frames, or a constant frame rate for some video editors);
  - adaptive mode, which records fewer frames for a while when a game needs the whole graphics
    card.
- **Saving:**
  - the recordings folder;
  - short messages in a corner of the screen ("Replay saved"), which never take focus from
    your game and never show in recordings;
  - a sound when recording starts and stops;
  - hiding Reccoon's windows while recording or live;
  - starting with Windows.
- **Shortcuts:** change any shortcut, or turn it off.
- **About:** Classic or Studio, and the look: **Simple** (the lightest) or **Fancy** (a blurred
  copy of your wallpaper behind the window).

## Shortcuts

| Shortcut | |
|---|---|
| **Alt+F9** | Start / stop recording |
| **Alt+F10** | Save instant replay |
| **Alt+F8** | Add a marker |
| **Alt+F7** | Pause / resume |

They work everywhere, also inside games. If another program already uses one, Reccoon tells you
on Home and on the Shortcuts page.

## When something doesn't work

**The recording is black.**
Protected video (Netflix and similar) always records black. A few games in exclusive full
screen do too: switch the game to borderless or windowed full screen.

**My game isn't in the Game capture list.**
Start the game, then press ↻ in the Edit window. If it's still missing, Windows doesn't know it
as a game: add it with **Screen… → Window** instead.

**A Screen or Game item is black.**
The program isn't running or is minimized. It shows again as soon as it's open, also in a
recording or stream that's running.

**I can't take a screenshot of Reccoon.**
While you record or are live, Reccoon hides its windows from all captures, screenshots
included. Stop first, or turn this off in **Settings → Saving**.

**The mixer says "Silent: muted on the headset?"**
Your microphone sends only silence. Check the mute switch on your headset or its cable.

**"Couldn't go live".**
Check the stream key in **Settings → Stream** (YouTube and Twitch keys can be reset on their
sites, and TikTok gives a new server and key every time). On YouTube, a stream must be set
up in YouTube Studio first.

**The PC test or a recording says a quality is too much.**
Pick the recommended quality on the Video page, or leave adaptive mode on so games stay smooth.

**Where are my settings and logs?**
Settings: `%APPDATA%\Reccoon\settings.json`. Logs: `%LOCALAPPDATA%\Reccoon\logs`. If you report a
problem on GitHub, attaching the log helps a lot.

**Command line.**
`reccoon-cli.exe` records, trims and compresses from a terminal, for scripts. Run
`reccoon-cli --help` for everything it can do.

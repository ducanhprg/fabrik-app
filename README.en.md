# Spotter

*[Tiếng Việt](README.md)*

Spotter watches your 3D printers on your own network: live status and camera on a dashboard,
alerts with a photo to your Telegram (or email) when a print starts, finishes, fails or gets stuck,
and controls (pause, resume, cancel, temperatures, light). Everything runs on your PC; nothing goes
through a cloud.

Works with **Snapmaker U1** and other **Klipper / Moonraker** printers, and **Bambu Lab** printers in
LAN mode. Windows only for now. It speaks Vietnamese unless switched to English (top right).

## Install

1. Download **`Spotter-<version>-windows.zip`** from the newest release under
   [Releases](../../releases/latest) and unzip it into a folder of its own (for example `Documents\Spotter`).
   Not Program Files: Spotter updates itself in its folder.
2. Double-click **`spotter.exe`**. Windows may say "Windows protected your PC": click
   **More info → Run anyway**. Allow it on the firewall prompt if you want to open the dashboard from
   your phone.
3. The dashboard opens in your browser (<http://localhost:8484>). Keep the black window open: closing it
   stops Spotter.
4. Click **Scan network** and add your printers.
   - **Bambu Lab:** turn on **LAN only** mode and **developer mode** on the printer, and type its
     **access code** (printer screen, network settings) when you add it. Keep `ffmpeg.exe` beside
     `spotter.exe`: the Bambu camera needs it.

The settings live in the `data` folder next to `spotter.exe` (your Telegram token and printer access
codes are in there: don't share that folder).

## Telegram alerts

Click **Set up Telegram** on the bar at the top of the dashboard (or **Notifications**) and follow its four steps:

1. **Make a bot:** in Telegram, message [@BotFather](https://t.me/BotFather), send `/newbot`, give it a name, and
   paste the token it sends you. Spotter shows the bot's name when the token is right.
2. **Choose where alerts go:** just you, a group (your family or print buddies), or a channel. **Open Telegram**
   takes you to the right place: press Start in the bot, or pick the group or channel to add the bot to.
3. **Find chats** and pick the one you want.
4. **Send test message**; when it arrives, click **Save**.

The bot token works like a password: don't share it.

## Updates

Spotter checks for a new version once a day (switch it off in the version button, top right). When
one is out, the dashboard shows a bar and your alert channel gets one message. Click **What's new**, then
**Install**: Spotter downloads it, checks it is a genuine release (it is signed), and restarts itself.
Install waits while a print is running. **Check now** in the same place checks straight away.

## Start with Windows (optional)

To have Spotter run in the background from boot, without the window: open a terminal **as
Administrator** in Spotter's folder and run

```
.\spotter.exe install
```

Then the dashboard is always at <http://localhost:8484>. `.\spotter.exe uninstall` undoes it (your
settings stay). Updates work the same way.

## If something is wrong

- **No printers found:** the PC and the printers must be on the same network. If they are on another
  subnet (for example the printer is on Wi-Fi and the PC on cable), add it under Notifications → extra
  subnets, or add the printer by its IP address.
- **No alerts:** a VPN can block Telegram; try with the VPN off. **Send test** in Notifications shows the error.
- **"Is Spotter already running?":** it is: another window or the service already has it running. The
  dashboard opens anyway.

`FFMPEG.txt` in the zip says which ffmpeg build is included and where its source is.

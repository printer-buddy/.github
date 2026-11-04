# Printer Buddy

A self-hosted monitor for Klipper 3D printers. It runs on a Raspberry Pi, a NAS, a home server or on a printer itself, finds the Moonraker printers on your network, and gives you one dashboard for all of them.

- **One dashboard for many printers:** status, temperatures, jogging, macros, files, the job queue and history, in a layout you can rearrange.
- **Cameras:** live view and snapshots, with an optional camera streamer for USB, Pi and network cameras.
- **AI failure watch:** looks at the camera during a print and warns you when it thinks the print has failed.
- **Notifications and timelapse:** alerts at the milestones you choose, sent to ntfy and Discord, and a timelapse of every print.
- **Share links:** let someone watch a print without giving them access to the rest of your setup.

## Pick what you install

Printer Buddy is made of parts, and you choose how heavy each one is. The installer asks about each in turn, and you can change any of them later.

| Part | Choices |
|---|---|
| Interface | advanced |
| AI detection | off, basic, heavy |
| Video | snapshots, live, timelapse |
| Notifications | basic, advanced |
| Remote access | off, on |
| Camera streamer | off, light, basic, advanced |
| Release channel | stable, nightly |

## Install

Run it on the same machine as Klipper and Moonraker, or on any other Debian-based computer on the same network as your printers (a Raspberry Pi, a NAS or a home server):

```bash
git clone https://github.com/printer-buddy/printer-buddy.git
cd printer-buddy
./install.sh
```

The first time you run it, the installer walks you through the choices above. Then open `http://<box-ip>:8080`.

## Coming soon

- **Full remote access:** open all of Printer Buddy from anywhere, with a login. Today, remote access is share links.
- **More printers:** Klipper is supported today, and support for more is being added over time.
- **32-bit AI:** a 32-bit version of the lite AI model, so AI detection works on 32-bit systems too.

## Help and documentation

- **Documentation:** https://printer-buddy.github.io/printer-buddy-docs
- **Found a bug or want a feature:** open an issue in the repository it belongs to, and the form will ask for what we need.
- **Security problems:** see [SECURITY.md](https://github.com/printer-buddy/.github/blob/main/SECURITY.md).

<a href="https://ko-fi.com/printerbuddy"><img src="https://ko-fi.com/img/githubbutton_sm.svg" alt="Support us on Ko-fi" height="60"></a>
## Repositories

| Repository | What it is |
|---|---|
| [printer-buddy](https://github.com/printer-buddy/printer-buddy) | The core app, the installer and the AI runtime. All releases are published here. |
| [print-buddy-ui](https://github.com/printer-buddy/print-buddy-ui) | The web interface |
| [print-buddy-notify](https://github.com/printer-buddy/print-buddy-notify) | Notifications |
| [print-buddy-timelapse](https://github.com/printer-buddy/print-buddy-timelapse) | Timelapses |
| [print-buddy-streamer](https://github.com/printer-buddy/print-buddy-streamer) | The camera streamer |
| [print-buddy-relay](https://github.com/printer-buddy/print-buddy-relay) | The Cloudflare worker behind remote access and share links |
| [printer-buddy-docs](https://github.com/printer-buddy/printer-buddy-docs) | The documentation |

Contributing: see [CONTRIBUTING.md](https://github.com/printer-buddy/.github/blob/main/CONTRIBUTING.md).

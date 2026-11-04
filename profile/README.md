# Printer Buddy

A self-hosted monitor for Klipper 3D printers. It runs on a Raspberry Pi, a NAS, a home server or on a printer itself, finds the Moonraker printers on your network, and gives you one dashboard for all of them.

- **One dashboard for many printers:** status, temperatures, jogging, macros, files, the job queue and history, in a layout you can rearrange.
- **Cameras:** live view and snapshots, with an optional camera streamer for USB, Pi and network cameras.
- **AI failure watch:** looks at the camera during a print and warns you when it thinks the print has failed.
- **Notifications and timelapse:** alerts at the milestones you choose, and a timelapse of every print.
- **Share links:** let someone watch a print without giving them access to the rest of your setup.

You pick which parts to install and how heavy each one is.

## Install

On a Debian or Raspberry Pi OS box on the same network as your printers:

```bash
git clone https://github.com/printer-buddy/printer-buddy.git
cd printer-buddy
./install.sh
```

Then open `http://<box-ip>:8080`.

Documentation: **https://printer-buddy.github.io/printer-buddy-docs**

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

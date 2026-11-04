# Contributing

Thanks for wanting to help with Printer Buddy.

## Before you start

- For a bug or a feature idea, open an issue in the repository it belongs to. The form asks for what is needed.
- For a bigger change, open an issue first so we can agree on it before you spend time on it.

## Which branch

The core, UI, notify and streamer repositories use two branches:

- **`nightly`** is where the work happens. Open your pull request against `nightly`.
- **`main`** is the stable branch. It is moved by the release workflow, so please do not open pull requests against it.

The timelapse, relay and docs repositories only have `main`, so use that one there.

## Making a change

1. Fork the repository and make your change on a branch of your own.
2. Focus on one feature per pull request.
3. Write a detailed description. Say what the change does, why it is needed, what you changed to do it, and how you tested it. Include screenshots for anything people can see.
4. Open the pull request and fill in the form.

## Where things live

| Repository | What to change there |
|---|---|
| `printer-buddy` | The core app, the installer and the AI runtime |
| `print-buddy-ui` | The web interface |
| `print-buddy-notify` | Notifications |
| `print-buddy-timelapse` | Timelapses |
| `print-buddy-streamer` | The camera streamer |
| `print-buddy-relay` | The Cloudflare worker for remote access and share links |
| `printer-buddy-docs` | The documentation |

## Security problems

Do not report these in a public issue. See [SECURITY.md](SECURITY.md).

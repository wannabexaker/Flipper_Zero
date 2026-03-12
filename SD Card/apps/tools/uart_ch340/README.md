# UART CH340

Versioned Flipper Zero UART terminal app for GPIO serial communication.

## Latest Version

- `v0.1.2`

Latest build:

- `v0.1.2/dist/uart_ch340.fap`

## What This App Does

- opens and closes the Flipper UART port
- configures baud rate
- configures data bits
- configures parity
- configures stop bits
- shows a live RX/TX console
- sends ASCII commands
- resends the last message from the console
- opens a quick reply editor from the console

## Important

This app is for UART over the Flipper Zero GPIO pins.

It is not a USB host app for connecting a CH340 USB dongle directly to the Flipper USB-C port.

## Folder Structure

- `v0.1.0/`
  First stable version snapshot.
- `v0.1.1/`
  Added custom console behavior and splash screen.
- `v0.1.2/`
  Added animated startup screen with auto-continue.

Each version folder includes:

- source files
- manifest
- icon assets
- `dist/` output

## Install

1. Open the latest version folder.
2. Copy the `.fap` file from `dist/` to your Flipper SD card.
3. Recommended app path on SD card:
   `/apps/GPIO/uart_ch340.fap`

## Wiring

- Flipper `TX` -> target `RX`
- Flipper `RX` -> target `TX`
- Flipper `GND` -> target `GND`

## Usage

1. Open the app.
2. Set `Baud`, `Data bits`, `Parity`, and `Stop bits`.
3. Set `Connect` to `Open`.
4. Open `Console`.
5. Use `Send ASCII` to type and send a message.
6. Inside the console:
   `Left` resends the last message.
   `Right` opens a reply editor.
   `Up/Down` scroll the log.

## Versioning Policy

Older versions are kept on purpose.

New changes are made in a new version folder instead of overwriting a previous working build.

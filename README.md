# Flipper Zero Apps

This repository contains custom Flipper Zero applications and versioned releases.

## Repository Layout

- `uart_ch340/`
  Versioned source snapshots and build outputs for the `UART CH340` app.

Each application folder may contain multiple version folders such as:

- `v0.1.0`
- `v0.1.1`
- `v0.1.2`

This keeps older working builds available while newer versions are developed.

## Current Apps

### `uart_ch340`

UART terminal app for Flipper Zero GPIO serial communication.

Features:

- UART open/close
- baud rate selection
- data bits, parity, stop bits
- live RX/TX console
- resend last message
- quick reply editor
- versioned builds

See the app-specific documentation in:

- `uart_ch340/README.md`

## Downloading a Build

If you only want to install an app on your Flipper, go to the app folder and use the latest versioned build from its `dist/` folder.

Example:

- `uart_ch340/v0.1.2/dist/uart_ch340.fap`

## Notes

- This repo is organized for end users and version tracking.
- Build caches, virtual environments, debug outputs, and unrelated local folders are ignored through `.gitignore`.

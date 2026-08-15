# Cod3Y Releases

Compiled release binaries for Cod3Y, a local-first, agent-native editor for macOS.

This repository contains **no source code**. It exists so that an installed
Cod3Y can find and verify its own updates, and so a first installation can be
downloaded without an account.

## Installing for the first time

1. Open the newest release under [Releases](../../releases).
2. Download `Cod3Y_<version>_universal.dmg` — one file for both Apple Silicon
   and Intel Macs.
3. Open it, drag Cod3Y into Applications, and launch it.

These builds are not signed by an identified Apple developer and are not
notarized, so macOS will refuse the first launch. Open **System Settings →
Privacy & Security**, find the line about Cod3Y being blocked, and press **Open
Anyway**. Once, per machine.

## Updating

Cod3Y checks this repository on startup and offers the update in-app. Every
package is signed, and a package whose signature does not verify is refused
rather than installed.

## What else is in a release

`Cod3Y.app.tar.gz` and its `.sig` are what the in-app updater downloads, and
`latest.json` is what tells it a new version exists. They are not meant to be
downloaded by hand.

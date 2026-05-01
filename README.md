# BLUprint Lite — Update Manifest

This repository publishes update metadata for **BLUprint Lite**. The
product source code lives in a separate private repository; this public
manifest lets every running install check for new versions without
needing GitHub credentials.

## Contents

- [`version.json`](./version.json) — current latest version + release notes.
  The running app polls this file on startup and surfaces an in-app
  update banner when it advertises a newer version than the user has
  installed.
- [`CHANGELOG.md`](./CHANGELOG.md) — user-facing release history. The
  banner's "Ver cambios" link points here.

## Shipping a new version

1. Push the new code to the (private) source repo.
2. Bump `version` in `version.json` here, refresh the `notes` and
   `date`, commit, push.
3. Add a corresponding `CHANGELOG.md` entry.

Within ~5 minutes (raw.githubusercontent.com cache TTL), every running
install sees the new version and offers a one-click update.

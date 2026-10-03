# FriendJoin updates

Signed Windows application updates for FriendJoin.

On an existing installation of FriendJoin 0.31 or later, use the **อัปเดต** (Update) button. The application downloads the latest release, verifies its ECDSA signature and SHA-256 checksums, waits for current account operations, saves the current settings, and restarts after installation.

Update packages replace only the five application files. Local `data`, Target/Random settings, Folder IDs, Config ID, API keys, profiles, proxy files, account lists and recovery records stay on the PC. No GitHub login is needed on receiving PCs. Failed installations roll back; after a power interruption use `Repair-Update.cmd` from the full installation folder.

This repository contains **update payloads only**. The full installation ZIP (including the owner's default proxy list and private profile) is distributed separately and is not uploaded here. Existing 0.30 or earlier users need the full 0.31 package once; keep their existing `data` folder in place.

Requires Windows and .NET 10 Desktop Runtime, as the existing portable application does. A release contains `update.json` and `FriendJoin-update-VERSION.zip`. Source archives automatically provided by GitHub are not installers.
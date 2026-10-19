# Cresard Desk releases

Built installers for **Cresard Desk**, the Windows desktop application Cresard
uses to run its own clients, quotations and invoices.

## This repository holds releases and nothing else

There is no source code here. The source lives in a private repository, and
nothing in this repository is needed to build the application.

## What a release contains

- `Cresard Desk_<version>_x64-setup.exe` - the installer, produced by the
  application's own release workflow.
- `latest.json` - the update manifest that an installed copy of the application
  reads to discover a newer version.

## About signatures

Two different things are called signing and only one of them is here.

Each release is signed with the **update signing key**. The application verifies
that signature before it will install an update, so a downloaded installer that
has been altered is refused rather than run. The matching public key is compiled
into the application.

The installer is **not** signed with a Windows code signing certificate. Windows
will therefore warn that the publisher is unknown. Choose "More info", then "Run
anyway". Windows code signing is a paid certificate and is not in place.

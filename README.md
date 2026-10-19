# Cresard Desk releases

Downloads for **Cresard Desk**, the Windows desktop application Cresard uses to
run its own clients, quotations and invoices.

Read this first. This repository holds releases and nothing else. There is no
source code here, and nothing in this repository is needed to build the
application. The source is not published.

The application is built for Cresard's own use. Its accounts are created by a
Cresard administrator, and there is no public sign up.

## What a release contains

- The **installer**. A Windows `.exe` whose name begins with `Cresard Desk` and
  ends with `-setup.exe`. Run it to install the application, or to upgrade an
  installed copy.
- The **update manifest**. A small JSON file that an installed copy reads to find
  out whether a newer version exists. Do not download it by hand.

## Installing

1. Download the newest installer, either from the [`installers`](installers)
   directory in this repository or from <https://desk.cresard.com/download>. A
   page on the Releases tab appears once a release has been published there.
2. Run it.

Windows will warn that the publisher is unknown, because the installer does not
carry a paid Windows code signing certificate. Choose **More info**, then
**Run anyway**.

The application asks for an email address and password when it starts. Those are
issued by a Cresard administrator.

## Updates

An installed copy checks this repository for a newer version and offers it.

Every release is signed with the update signing key, and the application verifies
that signature before it installs anything. An installer that has been altered
after publication is therefore refused rather than run. The matching public key
is compiled into the application.

## Licence

This is proprietary software. Copyright is held by Cresard, and all rights are
reserved.

No licence is granted by this repository other than the limited, revocable,
non exclusive right to download and run the installer, unmodified, for the
purpose it is intended for. You may not copy, modify, redistribute, sublicense,
sell or reverse engineer it, except where applicable law expressly permits that
and the permission cannot be excluded by agreement.

The full terms are in [LICENSE](LICENSE).

## Third party software

The application is built with open source components, among them React, Tauri,
Rust crates, Radix UI and the Inter typeface. Each is used under its own licence
and each keeps its own copyright.

Their licences and copyright notices are reproduced with the application and are
also published with every release. No component is used in a way that would place
the application under a copyleft licence.

## Trademarks

Cresard and Cresard Desk are trademarks of Cresard. Do not use the names or the
logo in a way that suggests endorsement or affiliation without written
permission.

## Security

Please report a security problem privately instead of opening a public issue.
Write to contact@cresard.com.

## No warranty

The software is provided as is, without warranty of any kind, express or
implied, including the warranties of merchantability, fitness for a particular
purpose and non infringement. Cresard is not liable for any claim, damages or
other liability arising from the software or its use.

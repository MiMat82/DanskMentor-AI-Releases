<p align="center"><img src="assets/marketing-lockup.png" alt="DanskMentor AI â€” by Novalon Learn" width="320"></p>

# DanskMentor AI Releases

AI-guided Danish learning and exam preparation.

by Novalon Learn

This repository holds release documentation, version manifests and download records for DanskMentor AI. **No installable packages have been published yet.**

- [Published releases](https://github.com/MiMat82/DanskMentor-AI-Releases/releases)
- [Application source repository](https://github.com/MiMat82/DanskMentor-AI)
- [Release policy](RELEASE_POLICY.md)
- [Unpublished manifest example](manifests/release-manifest.example.json)

| Target | Current availability |
| --- | --- |
| Desktop packages | No package published |
| Android APK | No package published |
| iOS IPA | No package published |

Each future release must list its actual files, source revision, SHA-256 checksums, supported platforms and verification results. A manifest example is documentation and does not create a software version or download.

The current engineering checkpoint adds **Create account** after initial setup and **Switch user**, with SQLite compiled into the software and separate saved learning for each person. Windows and WebAssembly builds pass, with **144 Rust tests, 21 account/restart checks and 43 baseline browser checks**. Both synthetic profiles kept their stable IDs and separate saved work after a real service restart. See the [local account checkpoint](manifests/local-accounts-checkpoint.json) for its exact source revision and build hashes. Earlier [GGUF tutor](manifests/local-gguf-tutor-checkpoint.json) and [initial Rust](manifests/rust-engineering-checkpoint.json) records remain preserved. Speaking acceptance, reviewed curricula, native/device qualification and distribution review remain separate gates. These records provide no installer, APK or IPA download.

DanskMentor AI is an independent learning aid. It does not issue official examination certificates or imply government endorsement. Software attribution is recorded in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

The later [account field guidance update](manifests/account-field-guidance-checkpoint.json) clarifies the separate username (3–64 characters) and new-password (at least 12 characters) requirements in English and Danish. Validation and stored credentials are unchanged. Windows and Wasm rebuilds, 144 existing Rust tests and five read-only browser checks pass. This is an unpublished engineering update with no installer or download assets.

The [Windows microphone callback fix](manifests/native-capture-checkpoint.json) continues recording after recoverable audio warnings and prevents overlapping capture teardown. It passes 149 desktop-feature Rust tests, including five synthetic native capture regressions, strict Clippy, Windows and Wasm builds, and a deliberately forced-red regression sensitivity check. The original device notification remains unknown; physical microphone operation and full speech acceptance remain unqualified. This checkpoint publishes no executable or download asset.

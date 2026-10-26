<p align="center"><img src="assets/marketing-lockup.png" alt="DanskMentor AI — by Novalon Learn" width="320"></p>

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

The current engineering checkpoint implements both the interface and backend in Rust. Windows and WebAssembly builds pass, with 72 Rust tests and 43 browser acceptance checks. This remains an unpublished local development build: live AI/speech, reviewed curricula, mobile qualification and distribution review are incomplete. See the [checkpoint record](manifests/rust-engineering-checkpoint.json) for the source revision and build hashes. No installer, APK or IPA is available from that record.

DanskMentor AI is an independent learning aid. It does not issue official examination certificates or imply government endorsement. Software attribution is recorded in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).

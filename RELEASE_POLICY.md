# Release policy

## Repository responsibilities

Application changes belong in [DanskMentor-AI](https://github.com/MiMat82/DanskMentor-AI). This public repository holds release records and approved product artwork. Installable binaries belong on the corresponding GitHub Release as assets; this repository does not contain the private application source, learner records, working documents, signing credentials or temporary files.

## Publishing an actual update

1. Identify the source commit and the version being released.
2. Produce each applicable desktop, APK or IPA artifact through its real build process. Record any platform that is unavailable and why.
3. Verify installation/startup and the supported workflows on the stated environment. Record the checks that actually ran and their results.
4. Complete the applicable content, security, privacy, dependency-license and signing checks. A successful source compilation alone does not establish an installable or releasable package.
5. Compute each final artifact's SHA-256 and byte size. Record the supported platform/architecture, package format and signing status.
6. Create a version manifest and release notes linked to the source commit. Attach the verified files and manifest to the actual release.
7. Read back the published release, download references and checksums. Preserve earlier release records; record corrections transparently.

Do not create an empty version tag, a placeholder binary or a successful-looking download entry for a package that does not exist. Example manifests remain explicitly unpublished. This initial documentation commit creates no software release.

## Manifest format

Manifest schema version `1` keeps the product version, release tag, source revision, publication time, targets and artifacts separate. The [example](manifests/release-manifest.example.json) deliberately uses null version/revision fields and empty artifact lists. Actual releases replace those unknowns with verified values and at least one real artifact.

An artifact record includes its filename, platform, architecture, package format, download URL, SHA-256, byte size, signing status and verification evidence. Release notes distinguish supported behavior, known limitations and platform availability.

## Assets and notices

The complete supplied marketing lockup is preserved unchanged at `assets/marketing-lockup.png`. Application packages derived from DeepTutor must preserve the applicable Apache-2.0 license, attribution and required third-party notices. Review the actual packaged dependency graph for each distribution; this repository's documentation does not certify that review.

No paid CI, signing service, automatic publishing workflow or public application deployment is configured by this bootstrap.

# Updates

About > Updates supports manual and optional startup checks, release notes, a visible Update available action, progress, cancellation, retry and explicit storage cleanup. An unavailable channel is reported as an error, not a successful update.

The official release channel is robertmartic/polyphoto on GitHub. No photos or credentials are sent. Downloads use HTTPS and SHA-256 digests from the official GitHub release API. This trusts the release account/service and is not an Authenticode signature.

Installed copies download a matching file-level delta only when every base file matches; otherwise they use the full package. The maintenance installer updates registration without another full payload. A helper verifies staged files, switches directories and rolls back on application/registration errors. Unsaved projects require Save / Don't save / Cancel before restart. Failed updates are never marked successful. A real installed-app update requires the owner's confirmation.

Portable copies check the same channel but show that setup or manual replacement is required. They never replace a registered installation.

About > Updates > Manage update storage shows recognized downloads and retained backups. Cleanup preserves active jobs, the latest verified backup, user documents, preferences and document recovery. An interrupted installation may require the full installer; keep backup folders until the app and documents are confirmed working.

0.1.0 is the full baseline: setup, portable ZIP, update manifest and maintenance installer. No public delta applies until a previous PolyPhoto release exists.

## Optional PolyHUB integration

This release supports the local PolyHUB protocol for coordinated updates. PolyHUB requests the existing application updater; download controls, save prompts, deltas/full fallback and rollback remain in this application. It also verifies the installed result. The app remains fully usable without PolyHUB. Setup, uninstall and update helpers coordinate maintenance to avoid concurrent changes.

Version 0.1.5 supplies a file-level delta from 0.1.2 when its installed files match the published base manifest. Older or modified copies use the full package.

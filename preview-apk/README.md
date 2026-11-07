# Morrow Android preview

This is a separate, installable WebView shell for previewing the Morrow interface on Android. It bundles the current static frontend from `static/` at build time.

The preview mocks only the authentication check and identity response so the home screen can open without a server. Other API-backed features are intentionally not simulated and will not persist data or provide real chat, memory, sync, reminders, or push functionality.

Builds are produced by the GitHub Actions workflow `.github/workflows/build-preview-apk.yml` as the artifact `morrow-songqi-preview-apk`. This package uses application ID `com.morrow.songqipreview` and can be installed alongside a separately packaged Morrow app.

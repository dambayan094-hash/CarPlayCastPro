# CarPlay Cast Pro

React + Vite web app wrapped with Capacitor for iOS.

## Build a real iOS IPA without owning a Mac

Use the included GitHub Actions workflow:

1. Upload the project contents to the root of a GitHub repository.
2. Open **Actions** → **Build iOS IPA**.
3. Click **Run workflow** (or push to `main`/`master`).
4. Download the `CarPlayCastPro-IPA` artifact when the workflow completes.

The workflow builds the iOS app on GitHub's macOS runner with Xcode. It does **not** generate a fake IPA or shell-script executable.

The resulting IPA is unsigned. Sideloading/signing depends on the tool and Apple signing requirements you use.

## Important

Wrapping a web app with Capacitor does not bypass Apple's CarPlay entitlements or restrictions. A real CarPlay integration must use Apple-supported APIs and capabilities.

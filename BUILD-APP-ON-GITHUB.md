# Get both apps without installing anything (GitHub builds them)

1. Make a free account at github.com and create a **new repository** (Private is fine).
2. Upload **everything inside the `presenter-app` folder** (including the hidden `.github` folder;
   if your file manager hides it, use GitHub Desktop or `git push`) and commit to `main`.
3. Open the **Actions** tab. Two builds start by themselves:
   - **Build Android APK** (phone remote) -> Releases page, tag `latest`
   - **Build Desktop App** (the Presenter app for your PC) -> Releases page, tag `desktop-latest`
   Each takes about 3-8 minutes. If one doesn't start: Actions -> pick it -> **Run workflow**.
4. Open the repo's **Releases** page:
   - PC: download **Presenter-Setup.exe** and run it (or **Presenter-Portable.exe**, no install).
   - Phone: open the Releases page on the phone and tap **PresenterRemote.apk**.

## First-run notes
- Windows may show "Windows protected your PC" (the app isn't code-signed): click **More info -> Run anyway**.
- Windows Firewall will ask about network access: allow **Private networks** so the phone can connect.
- Mac: right-click the app -> **Open** the first time.

## Connecting the phone
Open Presenter on the PC, click **Phone**, scan the QR code with the phone camera and choose
**Presenter Remote**. The PIN is in the QR code, so nothing to type.

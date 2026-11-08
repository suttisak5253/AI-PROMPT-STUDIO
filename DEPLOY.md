# Publish AI Prompt Studio

1. Open the repository Settings.
2. Select Pages.
3. Under Build and deployment, choose GitHub Actions.
4. The workflow publishes the standalone `index.html` from the repository root after each push to `main`.
5. When the deployment finishes, open the Pages URL shown in Settings → Pages or in the Actions deployment summary.

The app works as a static browser application. Projects are saved in the current browser's Local Storage; use Export JSON for backup and moving projects between devices.

AI video generation, external TTS, image upscaling, cloud media storage, and cross-device server sync are not connected in this MVP.

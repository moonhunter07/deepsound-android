# DeepSound DSP — Android APK build

This project is the original Google AI Studio React/Vite app wrapped with Capacitor.

## Build in GitHub Actions (no PC required)

1. Upload the whole project to a GitHub repository.
2. Open **Actions** → **Build DeepSound APK**.
3. Run the workflow with **Run workflow** (or push to `main`).
4. When the job finishes, open the workflow run and download the artifact **DeepSound-DSP-debug**.
5. Inside it is `app-debug.apk`, which can be installed on Android.

Package ID: `com.deepsound.dsp`

## Important

The current app is still a web/React DSP implementation. Capacitor makes it an installable Android app, but it does not automatically turn the Web Audio DSP into a native C++/Oboe audio engine. Background playback, Bluetooth routing, and system-level DSP behavior may therefore differ from a fully native audio app.

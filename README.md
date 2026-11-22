# CITY OF CRIME — starter build

## Play in Android browser
1. Upload this folder to a static host that serves HTTPS (for example GitHub Pages or Netlify).
2. Open the hosted `index.html` in Chrome on Android.
3. Use Chrome menu → Add to Home screen / Install app.

The project uses Three.js from jsDelivr, so the first load needs internet. The service worker caches the app shell; the Three.js CDN module may still need a first successful network load.

## Build an Android APK
Requires Node.js and Android Studio / Android SDK on a computer.

```bash
npm install
npm run build
npx cap add android
npx cap sync android
npx cap open android
```
Then in Android Studio choose Build → Build Bundle(s) / APK(s) → Build APK(s).

## Controls
- Desktop: WASD / arrow keys, Shift to run, E to interact.
- Mobile: left joystick to move; drag the open screen area to rotate camera; buttons for jump, interact, run, enter/exit car, next mission, and save.

## Current playable foundation
- Third-person 3D city scene with coastal water, beach, roads, buildings, palms, lighting and shadows.
- Character movement and camera.
- Drivable car with simple acceleration, steering and braking/reverse.
- Mission marker and ten mission steps with rewards.
- Local save, mobile touch controls, graphics/performance toggle.

This is the first playable vertical slice, not a finished AAA game. NPC AI, full mission scripting, traffic movement, advanced vehicle physics, audio, detailed character/vehicle assets and polished APK testing remain future development stages. The APK must be compiled with Android Studio; this environment cannot sign or compile a production APK.

# Speed Rush — Android-friendly 3D racing game

## Run on your computer

1. Install Node.js LTS from https://nodejs.org.
2. Extract this ZIP.
3. Open the `speed-rush` folder in VS Code.
4. Open **Terminal → New Terminal**.
5. Run:

   ```bash
   npm install
   npm run dev
   ```

6. Open the local URL Vite prints (usually `http://localhost:5173`).

## Test on your Android phone (same Wi-Fi)

1. Connect your phone and computer to the same Wi-Fi.
2. In the VS Code terminal, stop the server with `Ctrl+C`, then run:

   ```bash
   npm run dev -- --host 0.0.0.0
   ```

3. On Windows, open Command Prompt and run `ipconfig`.
4. Find your Wi-Fi adapter's **IPv4 Address**, for example `192.168.1.8`.
5. On your Android phone, open Chrome and visit `http://192.168.1.8:5173` using your own IPv4 address.
6. Tap **START RACE**. Hold **GAS ↑** to accelerate, use **← / →** to steer, and **BRAKE** to slow down.

If Windows Firewall asks, allow Node.js on your private network. The computer must stay on and the Vite server must keep running.

## Use it anywhere on your phone

To use the game away from your home Wi-Fi, deploy the project to a static hosting service such as Netlify or Vercel. Build it first:

```bash
npm install
npm run build
```

The production website files are created in the `dist` folder. Deploy the project through a supported Git repository integration or follow the host's current instructions for deploying a Vite project. After deployment, open its HTTPS URL in Chrome on Android. Use Chrome's menu (⋮) → **Add to Home screen** or **Install app**, if offered.

## Controls

- Desktop: W/↑ accelerate, S/↓ brake, A/D or ←/→ steer.
- Phone: hold GAS to accelerate; hold left/right to steer; hold BRAKE to slow down.

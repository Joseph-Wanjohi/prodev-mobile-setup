# README

A simple guide to get our React app running with Expo Go. Expo Go was already installed beforehand—no issues there!

## 1. Install Expo Go (already done)

- Visit https://expo.dev/go  
- Choose the latest SDK version  
- Install on your device via Google Play or App Store  
- Open the Expo Go app

## 2. Log in to Expo

- Open Expo Go  
- Sign up or log in with your existing account

## 3. Run the React App

```bash
git clone https://github.com/yourusername/your-react-app.git
cd your-react-app
npm install    # or yarn install
npm start      # or yarn start


## Objective

- Set up your first mobile application using the Expo Router template  
- Document the scaffolding process and understand the file structure

---

## Steps Followed

1. **Navigate to Project Directory**  
   ```bash
   cd prodev-mobile-setup
   ```
2. **Initialize Expo Project**  
   ```bash
   npx create-expo-app@latest .
   ```
   - Used the **Expo Router** template  
3. **Modify the Home Screen**  
   - Opened `app/(tabs)/index.tsx`  
   - Changed the default text from `Welcome!` to **First App Created**  
4. **Run & Test the App**  
   ```bash
   npx expo start
   ```
   - **iOS:** Scan QR code with the Camera app  
   - **Android:** Scan QR code with the Expo Go app  
5. **Reset the Application**  
   ```bash
   npm run reset-project
   ```

---

## Observations from `npm run reset-project`

- **File Changes Reverted:** All modifications to `app/(tabs)/index.tsx` and other source files were restored to their original scaffolded state.  
- **Dependencies & Lockfile:** `node_modules` was deleted and reinstalled; `package-lock.json`/`yarn.lock` remained intact.  
- **Cache Cleared:** Metro bundler cache was reset, ensuring a clean start on next `npx expo start`.  

---
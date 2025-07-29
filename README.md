# Expo + Maestro E2E Example

This project demonstrates how to use [Maestro](https://maestro.mobile.dev/) for end-to-end (E2E) testing in an [Expo](https://expo.dev) React Native app.

## Getting Started

### 1. Install Dependencies

```bash
yarn install
```

### 2. Start the Expo App

```bash
yarn expo start
```

Follow the Expo CLI instructions to run the app on an emulator, simulator, or device.

### 3. Install Maestro CLI

If you haven’t already, install Maestro globally:

```bash
curl -Ls "https://get.maestro.mobile.dev" | bash
```

Or with Homebrew:

```bash
brew install mobile-dev-inc/tap/maestro
```

### 4. Run Maestro E2E Tests

1. Make sure your Expo app is running on an emulator or simulator.
2. In a new terminal, run your Maestro flows:

```bash
maestro test <path-to-your-flow-file.yaml>
```

Replace `<path-to-your-flow-file.yaml>` with the path to your Maestro test flow.

## Project Structure

- `app/` – Main Expo app code (file-based routing).
- `eas.json` – EAS build configuration, including an `e2e-test` profile for E2E builds.
- `scripts/` – Project scripts (e.g., `reset-project.js`).
- `android/` – Native Android project (for advanced configuration).

## E2E Build Profile

The `eas.json` includes an `e2e-test` build profile for running E2E tests with Maestro. Example usage:

```bash
eas build --profile e2e-test --platform android
```

This will build an APK suitable for E2E testing.

## Learn More

- [Maestro Documentation](https://maestro.mobile.dev/)
- [Expo Documentation](https://docs.expo.dev/)

## Community

- [Expo on GitHub](https://github.com/expo/expo)
- [Maestro on GitHub](https://github.com/mobile-dev-inc/maestro)
- [Expo Discord](https://chat.expo.dev)

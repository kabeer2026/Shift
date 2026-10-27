# Shift

**Shift** is a high-performance, multi-account container desktop application designed to run multiple isolated Signal, WhatsApp, and Telegram accounts from one unified workspace.

---

## Key Features

- **Multi-Platform Support:** Manage Signal, WhatsApp, and Telegram accounts within one desktop application.
- **Multi-Account Containers:** Run multiple accounts for each supported platform simultaneously.
- **Isolated Session Data:** Every account uses its own isolated profile, preventing sessions, cookies, account data, and cache from leaking between profiles.
- **Fast Profile Switching:** Switch instantly between active account tabs from the Shift sidebar.
- **Persistent Sessions:** Signed-in accounts remain available after Shift is closed and reopened.
- **Bilingual Interface:** Supports English and Simplified Chinese.
- **Native Desktop Experience:** Clean, modern interface designed for smooth navigation between accounts.

---

## How It Works

Shift operates as a parent desktop application that manages separate account profiles for Signal, WhatsApp, and Telegram.

Signal accounts run through Shift’s bundled private Signal runtime, with a dedicated local profile directory for every account.

WhatsApp and Telegram run through a shared Microsoft WebView2 environment while maintaining completely separate named profiles for every account. This improves efficiency without sharing login sessions or profile data between accounts.

---

## Installation

### Prerequisites

- Windows 10 / 11 (64-bit)

All required application components, including the Microsoft Edge WebView2 Runtime, are included in the Shift installer.

### Getting Started

1. Go to the [**Releases**](https://github.com/kabeer2026/Shift/releases) page.
2. Download the latest `Shift-Setup.exe` installer.
3. Run the installer and select your preferred language.
4. Launch Shift using the desktop or Start Menu shortcut.

---

## Quick Start Guide

1. **Launch Shift:** Open the Shift application.
2. **Add an Account:** Click the **`+ Add Account`** button.
3. **Select a Platform:** Choose Signal, WhatsApp, or Telegram.
4. **Sign In:** Complete the platform’s normal account-linking or sign-in process.
5. **Switch Seamlessly:** Click any account tab in the sidebar to switch profiles instantly.
6. **Rename a Tab:** Assign a custom display name to identify each account easily.
7. **Delete a Profile:** Delete an account tab from the Shift interface when it is no longer required.

---

## Tech Stack & Architecture

- **Parent Host Application:** Manages account tabs, application windows, profile lifecycle, and persistent state.
- **Signal Runtime:** Uses Shift’s bundled private Signal runtime with a separate local profile directory for every Signal account.
- **WebView2 Environment:** WhatsApp and Telegram share one WebView2 environment while retaining isolated named profiles.
- **Profile Isolation:** Keeps the session data of every Signal, WhatsApp, and Telegram account separate.
- **Local Storage:** Account profiles and application state remain stored locally on the user’s computer.
- **Bundled Dependencies:** The installer includes Signal and the Microsoft Edge WebView2 Runtime required by Shift.

---

## Security & Privacy

- **No Shift Cloud Intermediary:** Shift does not operate a separate cloud service for handling account sessions or message content.
- **Isolated Account Profiles:** Login sessions and cached data remain separated between individual account profiles.
- **Local Data Storage:** Shift stores its profile data locally on the user’s computer.
- **Official Services:** Signal, WhatsApp, and Telegram continue communicating through their respective official services.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

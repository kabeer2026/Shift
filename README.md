# Shift

**Shift** is a high-performance, multi-account container desktop application designed to run multiple isolated Signal accounts simultaneously without performance degradation, lag, or session conflicts.

---

## Key Features

* **Multi-Account Containers:** Run multiple Signal instances side by side in completely isolated container environments.
* **Lag-Free Performance:** Optimized resource allocation ensures fast startup times and minimal memory overhead, even with several active accounts.
* **Isolated Session Data:** Keeps account storage, encryption keys, and cache strictly separated across containers to prevent data leaks.
* **Native Desktop Experience:** Clean, modern interface designed for smooth navigation between accounts.

---

## How It Works

Shift functions as a parent application that orchestrates lightweight container environments. Each container hosts a dedicated instance of Signal with its own isolated profile directory, allowing you to manage personal, work, and secondary accounts seamlessly from a single workspace.

---

## Installation

### Prerequisites
* Windows 10 / 11 (64-bit)

### Getting Started

1. Go to the **[Releases](../../releases)** page.
2. Download the latest release build (`Shift-v1.0.0.zip` or installer executable).
3. Extract and launch `Shift.exe`.

---

## Quick Start Guide

1. **Launch Shift:** Open the parent application.
2. **Add an Account:** Click the **`+ Add Account`** button on the sidebar to spin up a new isolated container.
3. **Link Signal:** Scan the QR code using the Signal app on your phone to authorize the instance.
4. **Switch Seamlessly:** Click between account tabs or use keyboard shortcuts to switch profiles instantly.

---

## Tech Stack & Architecture

* **Parent Host Application:** Manages container lifecycle, window framing, and process isolation.
* **Container Isolation:** Sandboxed user data directories ensuring independent session state and zero cross-account leakage.

---

## Security & Privacy

* **Zero Cloud Intermediary:** Shift operates locally on your machine. All network traffic routes directly between your local Signal instances and official Signal servers.
* **Local Data Encapsulation:** Session tokens and cached messages remain stored within their respective local container boundaries.

---

## License

Distributed under the MIT License. See `LICENSE` for more information.

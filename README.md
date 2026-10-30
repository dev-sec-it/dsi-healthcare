# DSI Care v2.0 - Clinic Management Software

Engineered and Published by **DEV SEC IT**  
Official Website: [https://devsecit.com](https://devsecit.com)  
GitHub Repository: [https://github.com/dev-sec-it/dsi-healthcare](https://github.com/dev-sec-it/dsi-healthcare)  
Release Version: `2.0.0` (30 October 2026)

---

## 1. Package Contents

This deployment directory contains the official production distribution of DSI Care v2.0:

| File | Description | Type |
|---|---|---|
| `DSI Care v2.0 Setup.exe` | Official Windows installer. Installs DSI Care to `%LOCALAPPDATA%\Programs\DSI Care` with Start Menu and Desktop shortcuts. | Windows Installer |
| `version.json` | Release manifest consumed by the GitHub automated update verification system. | Release Manifest |
| `LICENSE.md` | DEV SEC IT Freemium Software License Agreement. | Legal Agreement |
| `README.md` | Deployment guide and technical specifications. | Documentation |

---

## 2. Key Capabilities

- **Direct Doctor Gateway:** Software launches straight into the secure doctor authentication portal (`/login`) with automatic session resumption to `/appointments`. Marketing homepage is bypassed entirely in software mode.
- **OPD & Appointment Management:** Real-time patient appointment queuing, visited status tracking, consultation scheduling, and complete history logs.
- **Digital Prescription Suite:** Rapid prescription generation with dosage schedules, advice templates, test recommendations, and print/PDF export.
- **Chamber & Clinic Settings:** Complete inventory management for medicines, diagnostics, clinical tests, doctors, and staff roles.
- **Native Desktop Theme:** Windows MenuStrip navigation, native caption control (`-`, `[ ]`, `X`), and bottom StatusStrip displaying system readiness, network status, user credentials, and live clock.
- **Zero-Leak Single Binary Architecture:** Built with Rust (`tao` and `wry`). The Node.js production standalone bundle is embedded directly inside the binary via `include_bytes!`. No loose script files, source code, or plaintext secrets are exposed.
- **Hardened Security:** Right-click context menus are suppressed, DevTools shortcuts (`F12`, `Ctrl+Shift+I`, `Ctrl+Shift+J`, `Ctrl+U`) are blocked, and native devtools are disabled.
- **GitHub Update Verification:** Automatic background release check powered by `https://github.com/dev-sec-it/dsi-healthcare/releases`.

---

## 3. System Requirements

- **Operating System:** Windows 10 (1809+) or Windows 11 (64-bit)
- **Runtime:** Microsoft Edge WebView2 Runtime (included natively in modern Windows 10 and 11)
- **Memory:** 2 GB RAM minimum (4 GB recommended)
- **Storage:** 100 MB available disk space
- **Network:** Internet connectivity for remote API sync and cloud updates; local offline cache supported for standalone clinics.

---

## 4. Installation & Setup Guide

1. Download and run `DSI Care v2.0 Setup.exe`.
2. Follow the setup wizard to complete the installation.
3. The software installs directly into `%LOCALAPPDATA%\Programs\DSI Care` without requiring administrator privileges.
4. Launch DSI Care using the Desktop shortcut or from the Windows Start Menu under **DEV SEC IT**.
5. Log in with your registered mobile number or email and password to begin managing clinic operations.

---

## 5. Licensing

DSI Care v2.0 is licensed under the **DEV SEC IT Freemium Software License Agreement**.  
Refer to `LICENSE.md` in this directory for detailed licensing terms, permitted use, and commercial limitations.

For enterprise customizations, multi-chamber cloud deployments, or support:  
- **Publisher:** DEV SEC IT  
- **Website:** [https://devsecit.com](https://devsecit.com)  
- **Email:** info@devsecit.com


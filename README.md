# MOTO-HUB for iOS — releases

Pre-built IPAs and the AltStore source. **No source code here.**

MOTO-HUB projects a ride dashboard — map, navigation, speed, trip data — onto the
screen built into motorcycles whose dashboard speaks the EasyConn/Carbit
protocol: CFMOTO, Voge, Zontes, Moto Morini, Benelli, QJ Motor, Morbidelli.

Requires iOS 17 or later.

## Install

You need **AltStore Classic** — not AltStore PAL. See the note below if you
already have PAL.

**1. Get AltStore Classic.** Two ways, pick whichever suits you:

- **From AltStore PAL**, if you are in the EU, Japan or Brazil. PAL carries a
  notarized build of Classic that never expires, does not count against your
  three-app limit, and needs no computer to install or update. Get PAL at
  [altstore.io](https://altstore.io), then install AltStore Classic from inside it.
- **With AltServer** on a Mac or PC, which works anywhere. Download it from
  [altstore.io](https://altstore.io) and follow the setup guide for
  [macOS](https://faq.altstore.io/altstore-classic/how-to-install-altstore-macos)
  or [Windows](https://faq.altstore.io/altstore-classic/how-to-install-altstore-windows).

**2. Add this source** in AltStore Classic, under Browse → Sources → `+`:

```
https://raw.githubusercontent.com/vincenzobpt/MOTO-HUB-IOS-releases/main/source.json
```

**3. Install MOTO-HUB** from the source and open it.

Or skip AltStore entirely: download the IPA from [Releases](../../releases) and
sideload it with a tool of your choice, such as Sideloadly.

### "One or more apps are missing a marketplaceID"

If you add this source to **AltStore PAL** instead of Classic, PAL rejects it
with that message. Nothing is broken and there is nothing to fix in the source.

PAL is an Apple-sanctioned marketplace, so it installs only apps that Apple has
notarized, and notarization requires a paid Apple Developer account. These
builds are deliberately unsigned so that anyone can install them for free —
which is exactly what Classic is for. Add the source to AltStore Classic.

## What sideloading costs you

These builds are **unsigned**, and AltStore re-signs them on your device. That is
how sideloading works on iOS, and it comes with three limits that are Apple's,
not this app's. Better to know them now than in a car park.

- **You sign in with your own Apple ID.** AltStore uses it to create a free
  developer certificate. Your credentials go to Apple, not to us — we never see
  them and have no server.
- **The app stops working after 7 days** unless AltStore refreshes it. Refreshing
  takes seconds over Wi-Fi, but it has to happen. Refresh before a long trip.
- **A free Apple ID allows 3 sideloaded apps at a time**, across every app you
  have installed this way.

One thing that is easy to misread: the notarized AltStore Classic you can get
from PAL is itself exempt from the expiry and the three-app limit. Apps you
install *through* it are not. MOTO-HUB is still signed with your Apple ID, so
the 7 days and the limit apply to it.

A paid Apple Developer account (99 €/year) raises the 7 days to a year and the
limit to 100. Distributing through AltStore PAL would remove the Apple ID
requirement for you entirely — but it needs that same paid account on our side,
for Apple's notarization, so this app is not distributed that way today.

## One thing that will not work, and why

Joining the motorcycle's Wi-Fi automatically needs the Hotspot Configuration
entitlement, which a free Apple ID cannot carry. The app detects this, says so
once, and everything else works normally: join the motorcycle's network by hand
in Settings, then press Connect.

## Maps and routing

Maps, routing, search and weather use free public services — OpenFreeMap,
Valhalla, Photon, Open-Meteo, OpenStreetMap — and need no account. If you
navigate often you can add your own Stadia Maps key in Settings; leaving it
empty keeps the public server.

The motorcycle's Wi-Fi has no internet of its own, so map data travels over
mobile data.

## Status

The dashboard transport was rewritten from scratch for 1.3 and is young. If a
motorcycle connects but shows nothing, the in-app log now records what the
dashboard asked for and what it was actually sent — please attach it to an issue.

Not affiliated with CFMOTO or any motorcycle manufacturer.

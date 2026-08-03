# MOTO-HUB for iOS — releases

Pre-built IPAs and the AltStore source. **No source code here.**

MOTO-HUB projects a ride dashboard — map, navigation, speed, trip data — onto the
screen built into motorcycles whose dashboard speaks the EasyConn/Carbit
protocol: CFMOTO, Voge, Zontes, Moto Morini, Benelli, QJ Motor, Morbidelli.

Requires iOS 17 or later.

## Install with AltStore

Add this source:

```
https://raw.githubusercontent.com/vincenzobpt/MOTO-HUB-IOS-releases/main/source.json
```

Or download the IPA from [Releases](../../releases) and sideload it yourself.

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

A paid Apple Developer account (99 €/year) raises the 7 days to a year and the
limit to 100. AltStore PAL removes the Apple ID requirement entirely, but only
in the EU, Japan and Brazil, and only for apps notarized by Apple — this app is
not distributed that way today.

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

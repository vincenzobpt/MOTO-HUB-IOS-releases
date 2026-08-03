# MOTO-HUB for iOS — releases

Pre-built IPAs and the AltStore source. **No source code here.**

MOTO-HUB projects a ride dashboard — map, navigation, speed, trip data — onto the
screen built into motorcycles whose dashboard speaks the EasyConn/Carbit
protocol: CFMOTO, Voge, Zontes, Moto Morini, Benelli, QJ Motor, Morbidelli.

## Install with AltStore

Add this source:

```
https://raw.githubusercontent.com/vincenzobpt/MOTO-HUB-IOS-releases/main/source.json
```

Or download the IPA from [Releases](../../releases) and sideload it yourself.

## Worth knowing before you install

The builds here are **unsigned**. AltStore re-signs them with your own Apple ID,
which is normal — and has one consequence: joining the motorcycle's Wi-Fi
automatically needs an entitlement a free Apple ID cannot carry. The app detects
this, says so once, and everything else works. Join the motorcycle's network by
hand in Settings, then press Connect.

Maps, routing and search use free public services (OpenFreeMap, Valhalla,
Photon, Open-Meteo, OpenStreetMap) and need no account. The motorcycle's Wi-Fi
has no internet of its own, so map data travels over mobile data.

Requires iOS 17 or later.

Not affiliated with CFMOTO or any motorcycle manufacturer.

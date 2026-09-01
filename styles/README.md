# Map styles

These files exist so MOTO-HUB for iOS can download offline map areas.

MapLibre refuses to build an offline region from a style stored inside the app
("Relative file URLs cannot be used as offline style URLs"), so it is handed an
HTTPS copy instead. The app still *draws* with its own bundled copy; this one is
only ever read while a download is being planned, and usually not even then —
the app seeds MapLibre's database with its own bytes first.

Each file is byte-identical to the style shipped in the app build that
introduced it. **Never edit one in place.** A rider's downloaded areas were
built from exactly these bytes; changing them would quietly change what those
areas are supposed to contain. New style, new version directory.

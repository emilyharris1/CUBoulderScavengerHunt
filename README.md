
# CU Boulder AR Scavenger Hunt (Norlin + ATLAS)

This is a no-cost, WebAR starter built with A-Frame + AR.js (location-based). It anchors simple 3D markers at two CU Boulder spots:
- **Norlin Library** (main entrance area).
- **ATLAS / Visual Arts Complex** (near the CU Art Museum).

## Try it

1) Host the included `index.html` on **HTTPS** (GitHub Pages is easiest).  
2) Open it on your phone **on campus**.  
3) Allow **camera** and **location** when prompted.  
4) Look around; you should see labeled shapes floating over the real world where the targets are.

> Tip: Use Chrome on Android. On iPhone, Safari works but you may need to enable “Motion & Orientation Access” in Settings ▸ Safari.

## Change or add stops
Open `index.html` and update the two `gps-new-entity-place` attributes:
```html
<a-entity gps-new-entity-place="latitude: YOUR_LAT; longitude: YOUR_LON">
```
To get coordinates: long-press any point in Google Maps and copy the **decimal** lat/lon.

## Quick GitHub Pages
- Create a new public repo named, say, `cu-ar-hunt`.
- Upload `index.html` (and this README if you like).
- In **Settings ▸ Pages**, set Source = `main` / root.
- Open the Pages URL on your phone.

## Notes
- AR.js docs: Location-Based A‑Frame tutorial (AR.js 3.4.7) and `gps-new-camera` / `gps-new-entity-place` usage.
- Firefox mobile isn't supported for location-based AR due to device orientation limits; use Chrome (Android) or Safari (iOS).
- Accuracy: GPS may drift 5–20m outdoors. For best results, stand in open areas (not under trees/metal awnings) and give the sensor a few seconds.

Have fun!

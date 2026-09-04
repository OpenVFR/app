# OpenVFR

**Source code coming soon.**

OpenVFR is a free, open-source Electronic Flight Bag (EFB) for VFR pilots —
real-time airspace awareness, terrain and obstacle profiles, and aviation
charts, built entirely on open data. No account required, no paywalls, no
lock-in.

This repository is reserved and will be populated with the full source under
the [MIT License](./LICENSE) once the app is ready for its first public
release.

## ⚠️ Situational awareness only

OpenVFR is **not certified by any civil aviation authority** (FAA, EASA, or
otherwise) and must not be used as a primary means of navigation or
airspace compliance. It is intended strictly for pre-flight planning and
secondary, in-flight situational awareness.

The **pilot in command (PIC)** holds sole responsibility for flight safety,
airspace compliance, and the use of approved primary navigation sources.
Always cross-check against official, certified charts and NOTAMs (e.g. AIP,
eAIP, or your national aviation authority's published sources).

## Rollout

- **Web app** launches first — in **Sweden**, before expanding to the
  Nordics and other major European countries.
- **Android and iOS** apps follow shortly after the web app.

## Data & attribution

OpenVFR is built on the following data and map sources:

* **[aviationweather.gov](https://aviationweather.gov/)** (NOAA Aviation
  Weather Center) — METAR, TAF, and NOTAM data. US government, public
  domain. NOTAM coverage scope for non-US regions (including Sweden) is
  being verified — do not treat as a complete substitute for official
  national NOTAM/AIP sources.
* **[OpenSky Network](https://opensky-network.org/)** — live ADS-B air
  traffic data, via a registered OpenSky account (rate/credit limited).
* **[OpenAIP](https://www.openaip.net/)** — airspace and obstacle data.
  Licensed **CC BY-NC 4.0 — non-commercial use only.** This restricts
  commercial use of the combined app; see § License note below.
* **[OpenFlightMaps](https://www.openflightmaps.org/)** — VFR chart
  layers. Licensed ODbL.
* **[OpenStreetMap](https://www.openstreetmap.org/copyright)** (via
  Overpass API) — supplementary obstacles (masts, chimneys, water
  towers). Licensed ODbL.
* **[Protomaps](https://protomaps.com/)** (`@protomaps/basemaps`) —
  vector basemap tiles, fonts, and sprites. Licensed BSD-3-Clause.
* **ESRI** — satellite imagery basemap toggle. Proprietary / subject to
  ESRI's own terms of use — not open data; usage must comply with ESRI's
  licensing terms independently of this project's open-source status.

Each dataset carries its own license and attribution terms — see
individual source licenses before reuse.

> **License note:** OpenAIP's CC BY-NC 4.0 term applies to a component of
> this app's data, not its code. It restricts *commercial use of that
> data*, independent of the MIT-licensed source code. If OpenVFR or any
> fork is monetized, OpenAIP-derived layers may need to be replaced or
> licensed separately. This does not affect the code's MIT license, but
> does affect what a commercial deployment can legally display.

## Stay in the loop

- Website: [openvfr.org](https://openvfr.org)
- Join the waitlist / become an early adopter (especially in Sweden — beta
  testers wanted): [openvfr.org/#waitlist](https://openvfr.org/#waitlist)

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) once source lands — changes
affecting flight-critical calculations (fuel burn, weight & balance, true
airspeed, magnetic variation, great-circle/geodesic math) will require
test coverage before merge.

## License

Released under the [MIT License](./LICENSE). See the disclaimer above —
the license's standard "AS IS" warranty disclaimer applies in full; this
software carries no certification or guarantee of accuracy for flight use.

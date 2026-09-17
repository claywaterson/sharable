# Booking Leakage — Interactive Demo

**Status:** DEMO  
**Public demo:** https://booking-leakage.netlify.app/  
**Current demo build:** v0.2.0  
**Owner:** Clay Waterson  
**Public proof release:** v0.1.0

Booking Leakage is a synthetic private-aviation workflow demonstration showing how a material booking change can invalidate downstream assumptions and force a controlled review before confirmation.

## What the demo shows

A synthetic case moves through three layers:

1. **Diagnose** — identify workflow leakage and missing control conditions.
2. **Map** — align request version, quote validity, operator verification, client acceptance, payment condition, ownership and evidence.
3. **Standardize** — rehearse control ownership and expected outcomes before accepting an operating standard.

The public demonstration shows the operating pattern without exposing the complete commercial implementation.

## Demonstration boundary

- Synthetic records only.
- No live broker, operator, customer or payment systems are connected.
- No authentication or multi-tenant production boundary is claimed.
- Browser-local persistence is used in the current demo.
- The deterministic control model is a workflow demonstration, not a production brokerage booking engine.

## Architecture

See [docs/architecture.md](docs/architecture.md).

## QA evidence

The reviewed v0.2.0 release recorded:

- Domain rules: **7/7 passed**
- UI workflow tests: **3/3 passed**
- Event-demo browser gate: **13/13 passed**
- Production build: **passed**
- Browser page/console errors during the recorded rehearsal: **0**

See [docs/qa-summary.md](docs/qa-summary.md).

## What is intentionally not published

This public proof does not include production credentials, client data, private orchestration instructions, live integration configuration, commercial service-delivery logic, or the complete private implementation.

## Related

- Clay Waterson: https://claywaterson.com
- Live demo: https://booking-leakage.netlify.app/
- Public proof repository: https://github.com/claywaterson/sharable

## Provenance

Derived from the reviewed `CW_App_SeshCloud_BookingLeakage_20260916_v0.2.0` demo release. No third-party client data is included.

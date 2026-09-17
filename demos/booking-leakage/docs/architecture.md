# Public Architecture

## Purpose

Booking Leakage demonstrates a controlled booking-workflow pattern: when a material request changes, dependent assumptions should be revalidated before human confirmation.

## Current demo surface

The reviewed v0.2.0 build uses:

- React + Vite for the interface;
- synthetic booking fixtures;
- deterministic workflow/control evaluation;
- browser-local persistence;
- workspace JSON export/import;
- responsive desktop/mobile layouts;
- a three-layer Diagnose → Map → Standardize progression.

## State progression

```text
Tier 0 — Diagnose
        |
        v
Tier 1 — Map booking state + evidence
        |
        +-- hold while required conditions fail
        |
        v
Human review / mapping approval
        |
        v
Tier 2 — Standardize + rehearse controls
```

## Public control categories

The demo reasons about categories such as:

- current request/version alignment;
- quote validity;
- operator verification;
- client acceptance;
- payment condition;
- follow-up ownership;
- confirmation readiness.

## Production boundary

The demo does **not** establish production authentication, customer tenancy, server-side persistence, live CRM/booking synchronization, operator connectivity, payment-provider connectivity, production evidence storage, or confidential-data readiness.

Those belong to the authenticated SeshCloud delivery layer rather than this public proof.

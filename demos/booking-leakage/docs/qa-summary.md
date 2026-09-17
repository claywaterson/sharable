# QA Summary — Demo v0.2.0

**Source release:** `CW_App_SeshCloud_BookingLeakage_20260916_v0.2.0`  
**Release class:** Interactive synthetic demo  
**Production SeshCloud:** Not connected

## Recorded checks

| Check | Recorded result |
|---|---:|
| Domain rules | 7/7 passed |
| UI workflow tests | 3/3 passed |
| Production build | Passed |
| Event-demo browser gate | 13/13 passed |
| Browser page/console errors | 0 |

## Rehearsed path

1. Open synthetic CASE-0047.
2. Observe the hold state after a material passenger-count change.
3. Resolve current version, operator, acceptance and payment conditions.
4. Reach Ready for review.
5. Approve the Tier 1 map.
6. Open Tier 2, run the control rehearsal and accept the standards.
7. Reset the demo and confirm the canonical initial state returns.
8. Repeat the core progression in a fresh browser context.

## Limit

These checks validate the synthetic client demo. They do not validate production authentication, tenancy, live integrations or confidential-data handling.

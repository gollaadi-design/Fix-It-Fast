# Fix-It-Fast

Self-serve exception resolution prototype for delivery partners on quick-commerce platforms.

**Live prototype:** https://fix-it-fast-three.vercel.app/

## Problem
Delivery partners lose ~6 minutes per exception (GPS drift, COD blocks, store closures) because resolution requires a manual support call.

## Solution
A self-serve flow that resolves these exceptions on-device using:
- Geofence + AI photo verification for store closures
- UPI QR fallback for COD orders
- Ops dashboard tracking deflection rate and failed self-serve

## Projected Impact
- Handling time: 6 min → 45 sec
- Support deflection: 60%

## Product Decisions
- Caught a trust gap in my own design: v1 trusted the driver's self-report of arrival. Added geofence + photo verification to close the fraud vector.
- Separated driver UX from merchant/ops verification: driver is unassigned immediately, merchant dispute is async.

## Author
Adi Golla — Product Builder | B.Tech CSE '26 | Swiggy Product Ops
[LinkedIn](https://www.linkedin.com/in/adi-golla)

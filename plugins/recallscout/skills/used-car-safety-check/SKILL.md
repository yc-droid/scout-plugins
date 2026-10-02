---
name: used-car-safety-check
description: Run a complete safety check on a car someone owns or is about to buy. Use when the user shares a VIN, is buying a used car, or asks whether a specific car is safe, reliable or has open recalls.
---

To run a used-car safety check:

1. If the user gave a 17-character VIN, call `check_vehicle_by_vin`. Otherwise get the make, model and model year (ask only for what's missing) and call `get_vehicle_recalls`, `get_vehicle_complaints` and `get_safety_ratings`.
2. Lead with anything urgent: any recall flagged `do_not_drive` or `park_outside`, then the other recalls, newest first, each with the defect, the risk and the free remedy in one or two lines.
3. Summarize owner complaints as the top problem areas with counts, plus crashes, fires and injuries. Say clearly that complaints are unverified owner reports.
4. Give the NHTSA crash-test stars, or say the vehicle wasn't tested.
5. End with a short buyer checklist:
   - Confirm open recalls for this exact VIN at the NHTSA lookup link the tool returns, or ask a franchised dealer; safety recall repairs are free.
   - Ask the seller for repair records for each recall listed.
   - For the top complaint areas, what to inspect on a test drive.

Never say a specific car has or hasn't been repaired. Repair status per VIN isn't available here.

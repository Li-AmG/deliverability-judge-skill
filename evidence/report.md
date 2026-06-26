# Deliverability Judge Report

- Package: deliverability-judge@0.1.0
- Verdict: escalate
- Confidence window: conflicted
- Reason: bounce_pct 5.4 exceeds 2; inbox_placement_pct 62 below 90; high reputation conflicts with high bounce rate; high reputation conflicts with weak placement probe
- Recommendation action: none
- Evidence hash: none
- Postmaster source: postmaster.example.com/domain/example.net
- Bounce source: esp.example.com/metrics/bounce/2026-06-26
- Complaint source: esp.example.com/metrics/complaint/2026-06-26
- Placement source: seedlist.example.com/probe/def456
- Refusal reason: bounce_pct 5.4 exceeds 2; inbox_placement_pct 62 below 90; high reputation conflicts with high bounce rate; high reputation conflicts with weak placement probe
- Harness cases: sealed_healthy_signals_continue and contradictory_signals_escalate
- Effect boundary: read-only recommendation only; no send, throttle, mutation, state, or authority mint.


- runx doctor: success with 0 errors and 0 warnings.
- Local Windows harness blocker: receipt store os error 87; GitHub Actions Linux harness is configured to generate sealed receipts.

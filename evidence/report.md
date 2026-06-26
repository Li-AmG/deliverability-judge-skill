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

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:5f9afd29fa8f0352e70491f991f9b47e6156a9f714986d3a88b762b1a049a489
- GitHub Actions verify status: unknown

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:d33f1bbe1c784ffa7002c41bdd0c51e39e721844b2e7101597acf3a5afb9f931
- GitHub Actions verify status: unknown

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:203b519daa03ad5174333333e26d3bbe9021dd2219fe2fd609d2800d2f336bfb
- GitHub Actions verify status: unknown

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:a5a63141c11c5bc4b35912423642525614ef79b7df6d0ba1790a4e5994edb122
- GitHub Actions verify status: unknown

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:a75c794f20bcb01bd508db9f72d6604b5c499bb85065ea031fbbad979ac78632
- GitHub Actions verify status: unknown

- Summary: deliverability-judge is a read-only runx skill that fuses sealed postmaster, bounce, complaint, and placement-probe signals into a deliverability verdict, emits a continue recommendation only for healthy non-contradictory evidence, and escalates contradictory or incomplete inputs without sending, throttling, mutating, or minting authority.

- GitHub Actions harness status: passed
- GitHub Actions dogfood receipt_ref: runx:receipt:sha256:f954ce4145841b20cb2daf571e9a9585bde4050ea6b3f5115db8fd385f227cf6
- GitHub Actions verify status: unknown

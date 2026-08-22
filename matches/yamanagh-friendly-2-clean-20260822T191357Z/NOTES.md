# yamanagh friendly #2 — clean six, 90-30, 6-0 najamjad (2026-08-22, ~19:11 UTC)

Rerun on their rotated quick tunnel
(farming-ict-corporation-magnificent.trycloudflare.com). Identical scoreline
and shape to friendly #1: three thief survivals, three cop captures, zero
technicals, all six audits verified, per-window commits unchanged both
sides (ours 24e902c5/1001b063, theirs b10dd23a/fc267d67).

Deltas closed since #1:
- DECLARATION WRITTEN this time — they now send gpu "none" as a string, so
  the egress validator passed; artifacts.written counted all 14 files.
- Same digest as #1 (6fc49383...) — same game_uid, same outcomes, expected.

Still open (their side, known): their consensus loop again pushed
consensus_sha envelopes (~10 accepted 19:11:04-19:11:28, each logged
unknown-field + accepted); we do not echo, so their report's confirmed will
read false again. Their choice pending: read peer_sha256 from our mailed
result document (works today) or wait for our post-freeze echo.

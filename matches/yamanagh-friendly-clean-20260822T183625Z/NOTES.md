# yamanagh friendly #1 — clean six, 90-30, 6-0 najamjad (2026-08-22)

First completed series with yamanagh, on their Cloudflare quick tunnel
(sequence-burke-outlets-occur.trycloudflare.com), hints off on our side
(declared beforehand), practice redirect to yamandahle@gmail.com.

## Cross-check against their document (theirs_result_*.json)

MATCHES, both sides:
- game_uid 3bc536d1-e7bd-cd4f-ccfb-a2feee6bebb5 (pre-derived before play)
- totals 90-30, 6-0, winner najamjad, no ties, no technicals
- all six windows: roles, results, scores, winners identical
- per-window commits identical: ours thief 24e902c5 (w1/3/5) / cop 1001b063
  (w2/4/6); theirs cop b10dd23a (w1/3/5) / thief fc267d67 (w2/4/6) — all
  four verified as live HEADs on GitHub 2026-08-22 18:35 UTC
- games_played_including_this: najamjad 6 / yamanagh 4, agreeing documents
- settlement sha256 6fc49383... IDENTICAL digit-for-digit in both documents

Pattern: our thief survived 34 steps all three windows; our cop captured on
step 29 all three. Tokens 0 both sides (our hints off; their llm "template").

## Known deltas (neither disputes the outcome)

1. Their consensus records `sha_match: false, peer_sha256: null,
   confirmed: false` — ROOT-CAUSED 2026-08-22 evening — an expectation
   UNIQUE TO THEIR BUILD, not a defect of ours: their series-end audit messages carry
   a `consensus_sha` field (11 copies accepted 18:22:47-18:23:20 UTC, each logged
   by our inbox as `inbox.unknown_fields` and ignored), and they expect the
   peer's digest back the same way. Our envelope is strictly
   {sender, records, result_claim}; every other pairing this league
   (three counted + friendlies) confirmed mutual agreement by comparing
   result documents, no in-band echo, no confirmed:false ever. Both documents carry the equal sha 6fc49383..., their
   `results_agreed` is true, so nothing contradicts — but before any
   COUNTED with them default closure is THEY read peer_sha256 from our mailed
   result document like every other team; the in-band echo is a post-freeze
   courtesy only if their build cannot. Their statement of the false was
   accurate; the attribution is their protocol, not our pipeline.
2. OUR declaration artifact was never written: egress validator blocked it
   on their greeting's `hardware_spec.gpu_model: null` (schema wants str;
   their machine has no GPU and they sent null). Announced as
   artifact.skipped + artifacts.incomplete; all 13 other files fine. Fix is
   theirs to send "none" as a string — or ours post-freeze to coerce null.
   The result's links.declaration therefore dangles in THIS archive.
3. Their log_files name one combined per-side file; ours per-window. Their
   sub_games carry steps; ours don't. Cosmetic, outside the digest scope.

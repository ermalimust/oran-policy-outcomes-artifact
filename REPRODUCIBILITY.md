# Reproducibility scope

All file paths below refer to the extracted contents of [companion_sources.zip](companion_sources.zip), unless stated otherwise. The complete methods and tables are in [technical_supplement.pdf](technical_supplement.pdf).

This is a document and selected-analysis release. Rebuilding the PDF, recalculating retained output aggregates, rerunning decisions from normalized observations, independently verifying raw source joins, and repeating live experiments are different levels of reproduction.

| Material | Included and reproducible | Not reproduced by this bundle |
|---|---|---|
| S1-S5, S7-S10: model comparisons, recovery, sensitivity | Complete displayed rows and protected TeX hashes; document rebuild | Model generation, independent evaluation and bootstrap estimates from model inputs |
| S6: stress-condition definitions | Full fixed definitions in TeX and PDF | No additional numerical experiment is implied |
| S11: TRACTOR replay | Complete displayed rows; protocol description | Replay from TRACTOR raw data and replay code |
| S12: local processing | Complete displayed rows and timing-boundary description | Per-batch timing recalculation or new performance measurements |
| S13-S14: normal E2 cycles | Complete displayed outcomes and timings | Packet, worker and scheduler joins from the five-cycle raw capture |
| S15: asynchronous A1/E2 | Complete displayed outcomes; unchanged Figure S1 | Independent A1/E2 audit of nine episodes from raw messages/captures |
| S16: pending restoration | Six-row `data/pending_restore_counts.csv`, sufficient to recover the displayed aggregate | Re-establishing refusals and wire absence from all 18 episodes and bounded captures |
| S17: delivery timing | All 720 paired outcomes in `data/timing_grid_cells.jsonl` and 90 rows in `data/timing_grid_aggregate.csv`; the displayed operating point can be reaggregated | Re-evaluating the timing grid from its separate 2,125 normalized reports or rejoining its raw reports |
| S18 and Section 10 | Frozen 1,067 normalized reports, 48 actions, original evaluator/outcomes, plan and protocol; portable post-hoc driver reproduces all 12 cases and the weighted-mean diagnostic | Independent verification of normalization against full raw E2 bytes/source logs; an online restoration experiment |
| S19 and Section 11: local concurrency | All 48 runs, 13,260 measured event records and 1,020 final snapshots; frozen worker code, synthetic inputs, offline recalculation and new local runs. Follow `concurrency/README.md` inside the extracted bundle | RAN control-path capacity, network-scale throughput, independent-host reliability or a new radio experiment |
| Sections 4, 6 and 10: selected implementation parameters | Decoded granularity fields for all 1,067 reports; requested reporting/granularity settings, 48 local-send parameter sets, source hashes and implementation-audit locations. See `data/kpm_period_fields.csv` and `data/implementation_parameter_manifest.json` | Complete raw message/capture verification, independently rerunning the RAN, or standards-conformance certification |
| Section 2.2: modeled natural clearance | `data/natural_clearance_audit.json`, a byte-identical retained audit of no-withdrawal paths, actual versus latched harmful steps, and absence of action-induced harm at the scheduled withdrawal step | Compliance with every service limit, field outcomes, or attributing every disappearance of harm to withdrawal |
| Section 2.2: ten software lifecycle cases | Byte-identical `data/lifecycle_scenarios.csv` with individual conditions and checks; `data/lifecycle_scenario_summary.json` selects the two corresponding 10/10 metrics and records the full summary's source hash | Live E2 execution, network fault coverage or deployment reliability |
| Section 3.4: TRACTOR source cadence | Byte-identical `data/tractor_source_timing.csv` with median/p95/p99 adjacent timestamp gaps, larger-gap counts and maxima for the two source streams | Uninterrupted periodic delivery, transport latency or the separate 914 replay-window denominator |
| Figure S1 | Exact vector asset | Reconstructing the plotted trace from raw A1/E2 capture |
| Figure S2 | Exact vector asset; source-provenance paired-rule inputs/results are included | Plot-generation script and raw payload/source joins |

## Included analysis inputs

`data/posthoc/rlc_provenance/` includes exact retained normalized actions/reports, the formal plan, protocol, original paired result and unchanged evaluator. It also includes the original OCUDU provider source for the metric denominator; its separate license applies. The portable driver changes paths and neutral documentation, not the calculation.

The driver verifies every original action outcome before evaluating the additional 60% low predicate. The 60% predicate is retrospective: the live experiment had no such completion criterion. The 75 later fully post-application batches do not establish instantaneous physical truth at a shadow decision. The crossing-batch fit does not reveal a byte split at application.

Normalized `raw_header_ref`, `raw_payload_ref` and `source_provenance_refs` are traceability references. Those referenced raw captures/logs are not included. Their existence in JSON does not provide independent verification of the normalization step.

## What a fuller release would additionally need

- S1-S10: model generator, gate and independent evaluator; exact configurations/seeds; lifecycle implementation; reproduction entry point and pinned dependencies; retained model population/results or deterministic regeneration instructions. Paired bootstrap and common-recovery calculations must retain their original denominators.
- S11: replay implementation/configuration and the exact TRACTOR input selection/checksums, with the upstream dataset's distribution terms.
- S12: nine 512-record batch timing sets, local benchmark implementation, storage-size inputs and environment description. The 18,000-sample sequential result retains an aggregate, not individual timing rows; absent rows cannot be reconstructed as original observations.
- S13-S15: cycle/episode outputs, raw messages and captures, worker/scheduler/receiver logs, parsing and independent audit tools, plus pinned setup/configuration.
- S16: all 18 formal attempts, exact proposal and A1/worker events, packet capture/decoding evidence and independent completeness audit. Aggregate counts alone cannot prove command absence.
- S17: frozen timing plan, normalized timing reports/actions, sensitivity evaluator and normalization/audit dependencies. Raw payloads, source and scheduler logs are additionally required to independently verify source joins.
- Figure plotting: original plot-source tables and plotting scripts, if editable data-driven figure regeneration is required.

These items are intentionally outside this limited release. No new experiment, raw-data recovery, field-reliability estimate, or independent network deployment is implied by recomputing the included analysis.

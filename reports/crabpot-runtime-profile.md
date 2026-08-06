# Crabpot Runtime Profile

Generated: deterministic
Samples per command: 3

## Summary

| Metric                 | Value              |
| ---------------------- | ------------------ |
| Commands               | 9                  |
| P50 wall time          | 1262 ms            |
| Command P95 wall time  | 1288 ms            |
| Wall time basis        | command-median-p95 |
| Profile samples        | 27                 |
| RSS samples            | 1116               |
| CPU samples            | 1116               |
| Max peak RSS           | 130.4 MB           |
| Max RSS delta          | 101.4 MB           |
| Max CPU estimate       | 1753 ms            |
| Max harness heap delta | 4.8 MB             |

## Target OpenClaw Registry Surface

| Metric                 | Value      |
| ---------------------- | ---------- |
| status                 | ok         |
| configuredPath         | ./openclaw |
| compatRecords          | 0          |
| hookNames              | 44         |
| apiRegistrars          | 56         |
| capturedRegistrars     | 32         |
| sdkExports             | 302        |
| manifestFields         | 45         |
| manifestContractFields | 23         |

## Plugin Fixture Surface

| Metric                | Value |
| --------------------- | ----- |
| fixtures              | 8     |
| sourceFiles           | 708   |
| observedHooks         | 7     |
| observedRegistrations | 37    |
| observedSdkImports    | 296   |
| contractProbes        | 32    |
| issueFindings         | 39    |

## Boot And Memory Samples

| ID                     | Label                                           | Median wall | Max wall | Max peak RSS | Max RSS delta | CPU estimate | Heap delta | RSS/CPU samples | Exit codes |
| ---------------------- | ----------------------------------------------- | ----------- | -------- | ------------ | ------------- | ------------ | ---------- | --------------- | ---------- |
| node-boot              | Node boot                                       | 35 ms       | 36 ms    | 29 MB        | 0 MB          | 0 ms         | 0.4 MB     | 3/3             | 0          |
| fixture-inspection     | Fixture inspection                              | 1232 ms     | 1236 ms  | 123.8 MB     | 95.5 MB       | 1695 ms      | 4.8 MB     | 145/145         | 0          |
| compat-report-registry | Compatibility report plus target registry parse | 1262 ms     | 1273 ms  | 124.4 MB     | 96.3 MB       | 1740 ms      | 4.7 MB     | 150/150         | 0          |
| contract-capture       | Contract capture inventory                      | 1275 ms     | 1277 ms  | 126.1 MB     | 97.2 MB       | 1753 ms      | 4.4 MB     | 150/150         | 0          |
| synthetic-probe-plan   | Synthetic probe plan                            | 1278 ms     | 1279 ms  | 129.7 MB     | 101.1 MB      | 1734 ms      | 4.5 MB     | 150/150         | 0          |
| cold-import-readiness  | Cold import readiness                           | 1255 ms     | 1261 ms  | 130.4 MB     | 101.1 MB      | 1709 ms      | 4.4 MB     | 149/149         | 0          |
| workspace-plan         | Workspace execution plan                        | 1264 ms     | 1264 ms  | 129.7 MB     | 101.4 MB      | 1735 ms      | 4.4 MB     | 150/150         | 0          |
| platform-probes        | Platform and loader probes                      | 1288 ms     | 1299 ms  | 121.6 MB     | 92.2 MB       | 1752 ms      | 4.4 MB     | 153/153         | 0          |
| import-loop-profile    | Repeated cold import capture loop               | 567 ms      | 573 ms   | 64 MB        | 35.7 MB       | 305 ms       | 2 MB       | 66/66           | 0          |

## Category Rollups

| Category         | Commands | P50 wall | P95 wall | Max peak RSS | CPU estimate | RSS/CPU samples | Command IDs            |
| ---------------- | -------- | -------- | -------- | ------------ | ------------ | --------------- | ---------------------- |
| baseline         | 1        | 35 ms    | 36 ms    | 29 MB        | 0 ms         | 3/3             | node-boot              |
| fixture-scan     | 1        | 1232 ms  | 1236 ms  | 123.8 MB     | 1695 ms      | 145/145         | fixture-inspection     |
| target-registry  | 1        | 1262 ms  | 1273 ms  | 124.4 MB     | 1740 ms      | 150/150         | compat-report-registry |
| contract-capture | 1        | 1275 ms  | 1277 ms  | 126.1 MB     | 1753 ms      | 150/150         | contract-capture       |
| synthetic-probes | 1        | 1278 ms  | 1279 ms  | 129.7 MB     | 1734 ms      | 150/150         | synthetic-probe-plan   |
| cold-import      | 1        | 1255 ms  | 1261 ms  | 130.4 MB     | 1709 ms      | 149/149         | cold-import-readiness  |
| workspace-plan   | 1        | 1264 ms  | 1264 ms  | 129.7 MB     | 1735 ms      | 150/150         | workspace-plan         |
| platform-probes  | 1        | 1288 ms  | 1299 ms  | 121.6 MB     | 1752 ms      | 153/153         | platform-probes        |
| import-loop      | 1        | 567 ms   | 573 ms   | 64 MB        | 305 ms       | 66/66           | import-loop-profile    |

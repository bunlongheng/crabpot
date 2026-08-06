# Crabpot Import Loop Profile

Generated: deterministic
Mode: baseline-adjusted-cold-capture-loop
Entrypoint: test/fixtures/lazy-import-plugin.mjs

## Summary

| Metric                         | Value   |
| ------------------------------ | ------- |
| runs                           | 3       |
| baselineRuns                   | 3       |
| baselineFailCount              | 0       |
| p50WallMs                      | 106     |
| p95WallMs                      | 106     |
| p50PluginWallDeltaMs           | 0       |
| p95PluginWallDeltaMs           | 0       |
| maxPluginPeakRssDeltaMb        | 1.3 MB  |
| maxPluginCpuDeltaMsEstimate    | 5 ms    |
| maxPeakRssMb                   | 63.5 MB |
| maxCpuMsEstimate               | 83 ms   |
| baselineReferenceWallMs        | 107 ms  |
| baselineReferencePeakRssMb     | 62.2 MB |
| baselineReferenceCpuMsEstimate | 78 ms   |
| statSampleCount                | 12      |
| rssSampleCount                 | 12      |
| cpuSampleCount                 | 12      |
| capturedCount                  | 3       |
| failCount                      | 0       |

## Harness Baseline

| Metric                 | Value                                    |
| ---------------------- | ---------------------------------------- |
| mode                   | minimal-plugin-capture                   |
| runs                   | 3                                        |
| entrypoint             | .crabpot/import-loop/baseline-plugin.mjs |
| referenceWallMs        | 107 ms                                   |
| referencePeakRssMb     | 62.2 MB                                  |
| referenceCpuMsEstimate | 78 ms                                    |
| maxWallMs              | 108 ms                                   |
| maxPeakRssMb           | 63.1 MB                                  |
| maxCpuMsEstimate       | 90 ms                                    |
| statSampleCount        | 12                                       |
| failCount              | 0                                        |

## Samples

| Run | Status   | Captured | OpenClaw Import | OpenClaw Activate | Plugin Wall Delta | Plugin RSS Delta | Plugin CPU Delta | Raw Wall | Raw Peak RSS | Raw CPU Estimate | RSS/CPU samples | Exit |
| --- | -------- | -------- | --------------- | ----------------- | ----------------- | ---------------- | ---------------- | -------- | ------------ | ---------------- | --------------- | ---- |
| 0   | captured | 1        | n/a             | n/a               | 0 ms              | 1.3 MB           | 2 ms             | 102 ms   | 63.5 MB      | 80 ms            | 4/4             | 0    |
| 1   | captured | 1        | n/a             | n/a               | 0 ms              | 0 MB             | 5 ms             | 106 ms   | 61.8 MB      | 83 ms            | 4/4             | 0    |
| 2   | captured | 1        | n/a             | n/a               | 0 ms              | 0 MB             | 0 ms             | 106 ms   | 61.8 MB      | 71 ms            | 4/4             | 0    |

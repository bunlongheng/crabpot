# Crabpot Runtime Profile Diff

Generated: deterministic
Status: PASS
Strict: false

## Summary

| Metric        | Value |
| ------------- | ----- |
| Checks        | 10    |
| Fail          | 0     |
| Warn          | 1     |
| Pass          | 9     |
| Current runs  | 3     |
| Baseline runs | 3     |

## Checks

| Action | ID                              | Metric                 | Baseline | Current | Delta             | Percent | Message                                                        |
| ------ | ------------------------------- | ---------------------- | -------- | ------- | ----------------- | ------- | -------------------------------------------------------------- |
| pass   | profile.wall-p95                | p95WallMs              | 1273     | 1288    | 15                | 1.2%    | p95WallMs stayed within 50% regression threshold               |
| warn   | profile.peak-rss                | maxPeakRssMb           | 65.1     | 130.4   | 65.30000000000001 | -       | maxPeakRssMb regressed 65.30000000000001 over baseline         |
| pass   | profile.node-boot               | nodeBootWallMs         | 917      | 35      | -882              | -       | nodeBootWallMs stayed within 500 absolute regression threshold |
| pass   | registry.compatRecords          | compatRecords          | 19       | 0       | -19               | -       | registry surface delta is tracked as context                   |
| pass   | registry.hookNames              | hookNames              | 31       | 44      | 13                | -       | registry surface delta is tracked as context                   |
| pass   | registry.apiRegistrars          | apiRegistrars          | 40       | 56      | 16                | -       | registry surface delta is tracked as context                   |
| pass   | registry.capturedRegistrars     | capturedRegistrars     | 18       | 32      | 14                | -       | registry surface delta is tracked as context                   |
| pass   | registry.sdkExports             | sdkExports             | 307      | 302     | -5                | -       | registry surface delta is tracked as context                   |
| pass   | registry.manifestFields         | manifestFields         | 32       | 45      | 13                | -       | registry surface delta is tracked as context                   |
| pass   | registry.manifestContractFields | manifestContractFields | 16       | 23      | 7                 | -       | registry surface delta is tracked as context                   |

# Care Quality Commission
A manifest-only source for Care Quality Commission
https://www.cqc.org.uk/

## Configuration

| Input | Type | Description | Default Value |
|-------|------|-------------|---------------|
| `api_key` | `string` | API Key. Your CQC Primary Key. See https://www.cqc.org.uk/about-us/transparency/using-cqc-data#api for steps to generate one. |  |

## Streams
| Stream Name | Primary Key | Pagination | Supports Full Sync | Supports Incremental |
|-------------|-------------|------------|---------------------|----------------------|
| inspection_areas | inspectionAreaId | No pagination | ✅ |  ❌  |
| locations | locationId | DefaultPaginator | ✅ |  ❌  |
| providers | providerId | DefaultPaginator | ✅ |  ❌  |
| provider_locations | organisationId | No pagination | ✅ |  ❌  |
| locations_detailed | locationId | No pagination | ✅ |  ❌  |
| providers_detailed | providerId | No pagination | ✅ |  ❌  |

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                                                                                   |
|---------|------------|----------------------------------------------------------|-------------------------------------------------------------------------------------------|
| 0.0.31 | 2025-07-19 | [63454](https://github.com/airbytehq/airbyte/pull/63454) | Update dependencies |
| 0.0.30 | 2025-07-12 | [63085](https://github.com/airbytehq/airbyte/pull/63085) | Update dependencies |
| 0.0.29 | 2025-06-28 | [62142](https://github.com/airbytehq/airbyte/pull/62142) | Update dependencies |
| 0.0.28 | 2025-06-15 | [61078](https://github.com/airbytehq/airbyte/pull/61078) | Update dependencies |
| 0.0.27 | 2025-05-24 | [60662](https://github.com/airbytehq/airbyte/pull/60662) | Update dependencies |
| 0.0.26 | 2025-05-10 | [59797](https://github.com/airbytehq/airbyte/pull/59797) | Update dependencies |
| 0.0.25 | 2025-05-03 | [59320](https://github.com/airbytehq/airbyte/pull/59320) | Update dependencies |
| 0.0.24 | 2025-04-26 | [58743](https://github.com/airbytehq/airbyte/pull/58743) | Update dependencies |
| 0.0.23 | 2025-04-19 | [58286](https://github.com/airbytehq/airbyte/pull/58286) | Update dependencies |
| 0.0.22 | 2025-04-12 | [57601](https://github.com/airbytehq/airbyte/pull/57601) | Update dependencies |
| 0.0.21 | 2025-04-05 | [57125](https://github.com/airbytehq/airbyte/pull/57125) | Update dependencies |
| 0.0.20 | 2025-03-29 | [56575](https://github.com/airbytehq/airbyte/pull/56575) | Update dependencies |
| 0.0.19 | 2025-03-22 | [56124](https://github.com/airbytehq/airbyte/pull/56124) | Update dependencies |
| 0.0.18 | 2025-03-08 | [55383](https://github.com/airbytehq/airbyte/pull/55383) | Update dependencies |
| 0.0.17 | 2025-03-01 | [54860](https://github.com/airbytehq/airbyte/pull/54860) | Update dependencies |
| 0.0.16 | 2025-02-22 | [54218](https://github.com/airbytehq/airbyte/pull/54218) | Update dependencies |
| 0.0.15 | 2025-02-15 | [53880](https://github.com/airbytehq/airbyte/pull/53880) | Update dependencies |
| 0.0.14 | 2025-02-08 | [53400](https://github.com/airbytehq/airbyte/pull/53400) | Update dependencies |
| 0.0.13 | 2025-02-01 | [52938](https://github.com/airbytehq/airbyte/pull/52938) | Update dependencies |
| 0.0.12 | 2025-01-25 | [52174](https://github.com/airbytehq/airbyte/pull/52174) | Update dependencies |
| 0.0.11 | 2025-01-18 | [51777](https://github.com/airbytehq/airbyte/pull/51777) | Update dependencies |
| 0.0.10 | 2025-01-11 | [51251](https://github.com/airbytehq/airbyte/pull/51251) | Update dependencies |
| 0.0.9 | 2024-12-28 | [50495](https://github.com/airbytehq/airbyte/pull/50495) | Update dependencies |
| 0.0.8 | 2024-12-21 | [50218](https://github.com/airbytehq/airbyte/pull/50218) | Update dependencies |
| 0.0.7 | 2024-12-14 | [49546](https://github.com/airbytehq/airbyte/pull/49546) | Update dependencies |
| 0.0.6 | 2024-12-12 | [49008](https://github.com/airbytehq/airbyte/pull/49008) | Update dependencies |
| 0.0.5 | 2024-11-05 | [48368](https://github.com/airbytehq/airbyte/pull/48368) | Revert to source-declarative-manifest v5.17.0 |
| 0.0.4 | 2024-11-05 | [48329](https://github.com/airbytehq/airbyte/pull/48329) | Update dependencies |
| 0.0.3 | 2024-10-29 | [47897](https://github.com/airbytehq/airbyte/pull/47897) | Update dependencies |
| 0.0.2 | 2024-10-28 | [47671](https://github.com/airbytehq/airbyte/pull/47671) | Update dependencies |
| 0.0.1 | 2024-10-02 | [46315](https://github.com/airbytehq/airbyte/pull/46315) | Initial release by [@pabloescoder](https://github.com/pabloescoder) via Connector Builder |

</details>

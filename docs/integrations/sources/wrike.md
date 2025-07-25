# Wrike

This page guides you through the process of setting up the Wrike source connector.

## Prerequisites

- Your [Wrike `Permanent Access Token`](https://help.wrike.com/hc/en-us/community/posts/211849065-Get-Started-with-Wrike-s-API)

## Set up the Wrike source connector

1. Log into your [Airbyte Cloud](https://cloud.airbyte.com/workspaces) or Airbyte OSS account.
2. Click **Sources** and then click **+ New source**.
3. On the Set up the source page, select **Wrike** from the Source type dropdown.
4. Enter a name for your source.
5. For **Permanent Access Token**, enter your [Wrike `Permanent Access Token`](https://help.wrike.com/hc/en-us/community/posts/211849065-Get-Started-with-Wrike-s-API).

   Permissions granted to the permanent token are equal to the permissions of the user who generates the token.

6. For **Wrike Instance (hostname)**, add the hostname of the Wrike instance you are currently using. This could be `www.wrike.com`, `app-us2.wrike.com`, or anything similar.
7. For **Start date for comments**, enter the date in `YYYY-MM-DDTHH:mm:ssZ` format. The comments added on and after this date will be replicated. If this field is blank, Airbyte will replicate comments from the last seven days.
8. Click **Set up source**.

## Supported sync modes

The Wrike source connector supports on full sync refresh.

## Supported Streams

The Wrike source connector supports the following streams:

- [Tasks](https://developers.wrike.com/api/v4/tasks/)\(Full Refresh\)
- [Customfields](https://developers.wrike.com/api/v4/custom-fields/)\(Full Refresh\)
- [Comments](https://developers.wrike.com/api/v4/comments/)\(Full Refresh\)
- [Contacts](https://developers.wrike.com/api/v4/contacts/)\(Full Refresh\)
- [Folders](https://developers.wrike.com/api/v4/folders-projects/)\(Full Refresh\)
- [Workflows](https://developers.wrike.com/api/v4/workflows/)\(Full Refresh\)

### Data type mapping

Currencies are number and the date is a string.

### Performance considerations

The Wrike connector should not run into Wrike API limitations under normal usage. [Create an issue](https://github.com/airbytehq/airbyte/issues) if you see any rate limit issues that are not automatically retried successfully.

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                                                                |
| :------ | :--------- | :------------------------------------------------------- |:-----------------------------------------------------------------------|
| 0.3.32 | 2025-07-19 | [63646](https://github.com/airbytehq/airbyte/pull/63646) | Update dependencies |
| 0.3.31 | 2025-07-12 | [63201](https://github.com/airbytehq/airbyte/pull/63201) | Update dependencies |
| 0.3.30 | 2025-07-05 | [62742](https://github.com/airbytehq/airbyte/pull/62742) | Update dependencies |
| 0.3.29 | 2025-06-28 | [62203](https://github.com/airbytehq/airbyte/pull/62203) | Update dependencies |
| 0.3.28 | 2025-06-21 | [61781](https://github.com/airbytehq/airbyte/pull/61781) | Update dependencies |
| 0.3.27 | 2025-06-15 | [61216](https://github.com/airbytehq/airbyte/pull/61216) | Update dependencies |
| 0.3.26 | 2025-05-24 | [60751](https://github.com/airbytehq/airbyte/pull/60751) | Update dependencies |
| 0.3.25 | 2025-05-10 | [59974](https://github.com/airbytehq/airbyte/pull/59974) | Update dependencies |
| 0.3.24 | 2025-05-04 | [59533](https://github.com/airbytehq/airbyte/pull/59533) | Update dependencies |
| 0.3.23 | 2025-04-26 | [58942](https://github.com/airbytehq/airbyte/pull/58942) | Update dependencies |
| 0.3.22 | 2025-04-20 | [58579](https://github.com/airbytehq/airbyte/pull/58579) | Update dependencies |
| 0.3.21 | 2025-04-13 | [58047](https://github.com/airbytehq/airbyte/pull/58047) | Update dependencies |
| 0.3.20 | 2025-04-05 | [57380](https://github.com/airbytehq/airbyte/pull/57380) | Update dependencies |
| 0.3.19 | 2025-03-29 | [56851](https://github.com/airbytehq/airbyte/pull/56851) | Update dependencies |
| 0.3.18 | 2025-03-22 | [56317](https://github.com/airbytehq/airbyte/pull/56317) | Update dependencies |
| 0.3.17 | 2025-03-08 | [55589](https://github.com/airbytehq/airbyte/pull/55589) | Update dependencies |
| 0.3.16 | 2025-03-01 | [55118](https://github.com/airbytehq/airbyte/pull/55118) | Update dependencies |
| 0.3.15 | 2025-02-22 | [54501](https://github.com/airbytehq/airbyte/pull/54501) | Update dependencies |
| 0.3.14 | 2025-02-15 | [54030](https://github.com/airbytehq/airbyte/pull/54030) | Update dependencies |
| 0.3.13 | 2025-02-08 | [53573](https://github.com/airbytehq/airbyte/pull/53573) | Update dependencies |
| 0.3.12 | 2025-02-01 | [53080](https://github.com/airbytehq/airbyte/pull/53080) | Update dependencies |
| 0.3.11 | 2025-01-25 | [52430](https://github.com/airbytehq/airbyte/pull/52430) | Update dependencies |
| 0.3.10 | 2025-01-18 | [52020](https://github.com/airbytehq/airbyte/pull/52020) | Update dependencies |
| 0.3.9 | 2025-01-11 | [51400](https://github.com/airbytehq/airbyte/pull/51400) | Update dependencies |
| 0.3.8 | 2024-12-28 | [50752](https://github.com/airbytehq/airbyte/pull/50752) | Update dependencies |
| 0.3.7 | 2024-12-21 | [50321](https://github.com/airbytehq/airbyte/pull/50321) | Update dependencies |
| 0.3.6 | 2024-12-14 | [49794](https://github.com/airbytehq/airbyte/pull/49794) | Update dependencies |
| 0.3.5 | 2024-12-12 | [48237](https://github.com/airbytehq/airbyte/pull/48237) | Update dependencies |
| 0.3.4 | 2024-10-29 | [47801](https://github.com/airbytehq/airbyte/pull/47801) | Update dependencies |
| 0.3.3 | 2024-10-28 | [47668](https://github.com/airbytehq/airbyte/pull/47668) | Update dependencies |
| 0.3.2 | 2024-10-22 | [47234](https://github.com/airbytehq/airbyte/pull/47234) | Update dependencies |
| 0.3.1 | 2024-08-16 | [44196](https://github.com/airbytehq/airbyte/pull/44196) | Bump source-declarative-manifest version |
| 0.3.0 | 2024-08-09 | [43449](https://github.com/airbytehq/airbyte/pull/43449) | Refactor connector to manifest-only format |
| 0.2.12 | 2024-08-03 | [43260](https://github.com/airbytehq/airbyte/pull/43260) | Update dependencies |
| 0.2.11 | 2024-07-27 | [42804](https://github.com/airbytehq/airbyte/pull/42804) | Update dependencies |
| 0.2.10 | 2024-07-20 | [42292](https://github.com/airbytehq/airbyte/pull/42292) | Update dependencies |
| 0.2.9 | 2024-07-13 | [41796](https://github.com/airbytehq/airbyte/pull/41796) | Update dependencies |
| 0.2.8 | 2024-07-10 | [41360](https://github.com/airbytehq/airbyte/pull/41360) | Update dependencies |
| 0.2.7 | 2024-07-09 | [41278](https://github.com/airbytehq/airbyte/pull/41278) | Update dependencies |
| 0.2.6 | 2024-07-06 | [40954](https://github.com/airbytehq/airbyte/pull/40954) | Update dependencies |
| 0.2.5 | 2024-06-25 | [40330](https://github.com/airbytehq/airbyte/pull/40330) | Update dependencies |
| 0.2.4 | 2024-06-22 | [40033](https://github.com/airbytehq/airbyte/pull/40033) | Update dependencies |
| 0.2.3 | 2024-06-06 | [39224](https://github.com/airbytehq/airbyte/pull/39224) | [autopull] Upgrade base image to v1.2.2 |
| 0.2.2 | 2024-05-28 | [38663](https://github.com/airbytehq/airbyte/pull/38663) | Make connector compatible with Builder |
| 0.2.1 | 2024-04-30 | [31058](https://github.com/airbytehq/airbyte/pull/31058) | Changed last_records to last_record. Fix schema for stream `workflows` |
| 0.2.0 | 2023-10-10 | [31058](https://github.com/airbytehq/airbyte/pull/31058) | Migrate to low code. |
| 0.1.0 | 2022-08-16 | [15638](https://github.com/airbytehq/airbyte/pull/15638) | Initial version/release of the connector. |

</details>

# Burrow Plug connectors

Public, declarative connector catalog for [Burrow Plug](https://github.com/NightShaman/Burrow-Plug). No host runtime, server, executable connector, accounts, credentials or secrets are included.

The curated catalog at `catalog/index.json` lists Outlook Calendar as a read-only Microsoft Graph connector. Browsing this index does not install a connector or grant access: review and install its manifest explicitly in Burrow Plug, then consent to features and permitted agents.

Use the pinned catalog URL after this source is publicly published and its raw bytes verified:

`https://raw.githubusercontent.com/NightShaman/Burrow-Plug-Connectors/v2026.11.25/catalog/index.json`

The manifest is `connectors/outlook-calendar.json`, published at the matching pinned raw URL in the catalog. Its exact-file SHA-256 is `de497d368a11762ac95e4eba7683a31a7dc6dfbfd75a843c691a8b2519bbf371`. Check with `sha256sum connectors/outlook-calendar.json`. Do not retarget the `v2026.11.25` tag after publication; future content belongs under another version/tag with a fresh digest.

To author your own manifest or catalog, consult the [Burrow Plug connector format](https://github.com/NightShaman/Burrow-Plug/blob/main/docs/connector-format.md). Never place API keys or personal tokens in public JSON. The host validates a manifest before installation and enforces explicit consent.

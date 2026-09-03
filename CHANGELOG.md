# Changelog

## [1.4.0] - 2026-09-03

### Added

- The Signature Record surface: `GET`, `PUT` and `PATCH` on `/signature/{signature_id}/record`, letting a Partner read and update the Record attached to a Signature. A Record carries `custom_fields` (creator-defined display metadata), share-state and distribution fields, and optional `licensee` / `asset_source_id` fields.
- Optimistic concurrency on Record writes via `ETag` / `If-Match`, and a machine-readable validation-error contract that names the offending field and a closed `reason` code instead of only a free-text message.
- A lookup job result may now include `guidance` (a coarse verdict on how to treat the matched content) and the disclosed `record`, when the caller is entitled to it.

## [1.0.0] - 2025-XX-XX

### Added

- Initial release

[1.4.0]: https://github.com/Sasha-ApS/apis/releases/tag/v1.4.0
[1.0.0]: https://github.com/Sasha-ApS/apis/releases/tag/v1.0.0

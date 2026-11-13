# Redistribution policy - third-party data

Version 3.1, effective 2026-11-01. Applies to every third-party data shard in the demo sample pack.

## Allowlist

A shard may ship in the published pack only when the licence declared by its upstream collection is one of:

- Apache-2.0
- MIT
- ODC-BY
- CC-BY-4.0

## Withholding

Any other licence - including share-alike, non-commercial, no-derivatives, research-only, "other", unspecified or
missing licences - means the shard must be withheld from the published pack.

## Evidence rules

1. The authoritative licence is the one declared in the upstream collection's own repository metadata. Licence values
   copied into intake records are not authoritative.
2. A shard's upstream collection must be confirmed from its record schema (field names and value shapes), not from a
   similar name or from the team that published it.
3. Intake sign-offs recorded before this policy version are administrative records only. They do not waive the
   allowlist above.
4. The release notice must list only the shards that are permitted to ship. Withheld shards are reported to the release
   manager and tracked in the pack repository.

# Cinder-2 demo sample pack (staging)

Staging repository for the third-party data shards that ship inside the public Cinder-2 demo sample pack.

## Layout

- `data/` - one JSON Lines shard per upstream collection. Each shard is a resampled export of a few dozen records.
- `intake/` - intake and attribution records kept by the data team.
- `pack_manifest.json` - shard inventory used by the packaging job.
- `POLICY.md` - the redistribution policy that applies to every third-party shard.

## Export notes

The export tooling dropped the upstream identifiers and the upstream licence metadata from every shard. Field names
and value shapes were preserved from the original record schema, so a shard's origin can be confirmed by comparing its
fields and sample values against the upstream collection's published schema.

Shards were assembled from publicly available dataset collections on the Hugging Face Hub published by
HuggingFaceTB, HuggingFaceH4, allenai and openai.

The packaging job tars the **entire `data/` directory**. Every shard present here is part of the published pack.

The intake ledger predates the current redistribution policy and is kept as a historical record; it does not substitute
for a licence confirmation against the upstream collection.

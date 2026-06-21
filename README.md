# Dota2 Mechanism Ontology Dist

This repository stores the compiled `dist/` artifacts for the Dota 2 mechanism ontology project.

## Contents

- `dist/hero_profiles.json` - derived hero profiles
- `dist/item_profiles.json` - derived item profiles
- `dist/skills.json` - structured skill-layer ontology data
- `dist/relation_edges.json` - cross-entity relation edges
- `dist/indexes.json` - lookup indexes for profiles, traits, and edges
- `dist/retrieval_blocks.json` - RAG-ready retrieval blocks
- `dist/README.md` - retrieval block type summary

## Intended use

These files are the runtime-facing outputs of the ontology pipeline.

- Edit source knowledge in the upstream ontology project.
- Rebuild the `dist/` artifacts there.
- Sync the refreshed `dist/` directory into this repository.

Application code should read from `dist/` rather than from the source markdown and rule files.

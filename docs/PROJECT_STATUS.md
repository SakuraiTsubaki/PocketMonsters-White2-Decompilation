# Project Status

**Current stage:** Public-source survey and reconstruction baseline

This project currently assumes no local retail ROM baseline is available. Work therefore starts from public official material, preservation metadata, technical implementations, reverse-engineering research, and independently published evidence.

## Current baseline policy

- Japanese retail release is the canonical starting point for comparison.
- Every official regional/language/territory/revision target is tracked independently.
- White 2 is not merged with Black 2, Black, or White.
- Black 2 archive counts are not copied into White 2 by assumption.
- Unknown fields remain `TBD`/`Unknown`; no revision, hash, offset, or build identity is invented.
- Public hashes and catalogue metadata are reference evidence until independently verified under `VERIFICATION.md`.
- Research is integrated only when committed to GitHub; retail ROM binaries remain excluded.

## Version inventory status

- [x] Japanese product identity and official launch date documented (`IRDJ`, 2012-06-23).
- [x] Major US/Australia/Europe/Korea product-code targets seeded.
- [x] Separate European English/French/German/Italian/Spanish targets recorded.
- [x] Hong Kong/Taiwan/Canada/New Zealand/other served-market questions added as explicit research targets.
- [x] Japanese Rev 0 / Rev 1 ambiguity recorded instead of assumed away.
- [ ] Resolve exact Japanese launch-retail revision with independent cartridge/header evidence.
- [ ] Enumerate every revision for every regional build.
- [ ] Independently verify public-reference hashes.
- [ ] Complete territory/packaging variants and official distribution channels.

## Technical reconstruction progress

- [x] Repository policy, asset workflow, verification rules, and long-term structure established.
- [x] Public-source survey policy added.
- [x] Regional survey matrix added.
- [x] Evidence-backed NARC/NitroFS path catalog added (`docs/NARC_PATH_CATALOG.md`).
- [x] Machine-readable NARC path inventory added (`manifests/narc-paths.csv`).
- [x] Record BW → B2W2 path relocation for scripts, trainers, overworlds, and encounters.
- [x] Preserve the legacy PPRE B2W2 trainer/encounter mapping conflict instead of silently inheriting it.
- [x] Record B2W2-specific path leads for ZoneData, egg moves, PWT, Hidden Grotto, shops, trades, trainer graphics, and move animations.
- [ ] Find White 2-specific archive/file-tree census preservation evidence.
- [ ] Resolve Japanese launch revision before treating any paired-version structure as canonical Japan baseline.
- [ ] Establish which exact White 2 region/revision each B2W2 public tool/research source tested.
- [ ] Document executable and section layout.
- [ ] Map ARM9, ARM7, overlays, symbols, functions, and major subsystems.
- [ ] Document game-data formats and resource containers at record/field level.
- [ ] Reconstruct scripts, events, and behavior.
- [ ] Reconstruct asset pipelines and metadata.
- [ ] Fully document B2W2-specific systems (PWT, Pokéstar Studios, Join Avenue, Hidden Grotto, Medal, Memory Link, Key System, Funfest Missions, White Treehollow, difficulty modes).
- [ ] Add reproducible tooling where evidence and lawful inputs permit.
- [ ] Add automated verification where practical.

## Current technical baseline

B2W2-specific research supports White 2 path leads for text, maps/ZoneData, personal data, moves, learnsets/evolutions, scripts, trainers, overworld/events, encounters, trades, Hidden Grotto, PWT, shops, and trainer graphics. Unlike Black 2, the public Project Pokémon Raw DB index does not expose a White 2 tree, so White 2 member counts remain `TBD` instead of inheriting Black 2 counts.

Independent B2W2 trainer and encounter research also exposes a legacy PPRE conflict: trainer metadata/parties are `/a/0/9/1` and `/a/0/9/2`; overworld/event data and encounters are `/a/1/2/6` and `/a/1/2/7`.

## Verification levels

- **Unverified** — a proposed/imported claim not independently checked against a project target.
- **Observed** — confirmed directly in a specific target build, executable, extracted file, or runtime observation.
- **Reproduced** — recreated using documented steps, tooling, inputs, and target information.
- **Matched** — reconstructed output satisfies a defined exact-match criterion.

Research documents may additionally mark evidence as corroborated, direct technical, single-source, structural-only, or conflicted without promoting project-level verification.

## Next milestones

1. Resolve Japanese `IRDJ` launch revision identity.
2. Find White 2-specific archive census evidence and establish tested build identities behind public tools.
3. Expand high-value NARCs into record/field structures: personal data, moves, learnsets/evolutions, trainers, encounters, scripts, ZoneData/maps, Hidden Grotto, PWT, and shops.
4. Continue Japanese-baseline-to-region comparison at actual resource/data level.
5. Keep `VERSIONS.md`, `REGIONAL_SURVEY_MATRIX.md`, `NARC_PATH_CATALOG.md`, manifests, and this status synchronized.
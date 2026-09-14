# Regional Survey Matrix — Pokémon White 2

## Purpose

Track every officially released regional, territorial, language, packaging, and revision target of Pokémon White 2 against the original Japanese release baseline.

The matrix is evidence-first. Use `Unknown` or `TBD` when a field has not been verified.

## Baseline policy

- Baseline axis: original Japanese retail release.
- The exact Japanese launch revision is currently unresolved.
- Every non-Japanese build is compared directly against the Japanese baseline once that baseline revision is established.
- Non-Japanese builds are also cross-compared where necessary.
- Revisions are separate records.
- Language, territory, cartridge identity, release date, revision, packaging, and technical differences must not be conflated.

## Build inventory

| Record ID | Version | Territory / market | Language | Release date | Revision | Product / cart code | Known hashes | Evidence status | Sources |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| WHITE2-JP-BASE | White 2 | Japan | Japanese | 2012-06-23 | **TBD — Rev 0/Rev 1 launch-baseline question** | `TWL-IRDJ-JPN` / `IRDJ` | TBD | Official release confirmed; revision unresolved | Nintendo JP; Pokémon official; No-Intro preservation research |
| WHITE2-US-EN | White 2 | United States | English | 2012-10-07 | Unknown | `TWL-IRDO-USA` / `IRDO` | Unknown | Product/release catalogued | Nintendo regional release data; GameFAQs |
| WHITE2-AU-EN | White 2 | Australia | English | 2012-10-11 | Unknown | `TWL-IRDO-AUS` / `IRDO` | Unknown | Product/release catalogued | GameFAQs |
| WHITE2-EU-EN | White 2 | Europe | English | 2012-10-12 | Unknown | `TWL-IRDO-EUR` / `IRDO` | Public reference: CRC32 `b4416cec`; MD5 `51e380ed94bd5c70a9b46e3966f2cf88`; SHA-1 `a6c7e035063c6830d5ef7a28edf9152f1c3f59bf` | Release/product identity corroborated; bytes not project-verified | Nintendo Europe; GameFAQs; GameTDB |
| WHITE2-EU-FR | White 2 | France / Europe | French | 2012-10-12 | Unknown | `TWL-IRDF-FRA` / `IRDF` | Unknown | Product/release catalogued | GameFAQs; preservation catalogues |
| WHITE2-EU-DE | White 2 | Germany / Europe | German | 2012-10-12 | Unknown | `TWL-IRDD-NOE` / `IRDD` | Public reference: CRC32 `107b8669`; MD5 `40e4009ac3306dd18d04764d833a1595`; SHA-1 `4ed37674d2a09db4573bf579d2cc89c60794b59c` | Product/release catalogued | GameFAQs; GameTDB |
| WHITE2-EU-IT | White 2 | Italy / Europe | Italian | 2012-10-12 | Unknown | `TWL-IRDI-ITA` / `IRDI` | Unknown | Product/release catalogued | GameFAQs; preservation catalogues |
| WHITE2-EU-ES | White 2 | Spain / Europe | Spanish | 2012-10-12 | Unknown | `TWL-IRDS-ESP` / `IRDS` | Public reference: CRC32 `44e04b67`; MD5 `5fdb174c0e2a4ab9305373b9e90d2664`; SHA-1 `bf65769c43cd4db26f88c76f7aeee201c9322f0e` | Product/release catalogued | GameFAQs; GameTDB |
| WHITE2-KR | White 2 | South Korea | Korean | 2012-11-08 | Public catalogue: v0; project verification pending | `TWL-IRDK-KOR` / `IRDK` | Public reference: CRC32 `cf895342`; MD5 `4a7a098d122b24d04c2b2d6635db120f`; SHA-1 `57ce8d933ab593d05ce217b2a2e03e41979f5845` | Product/release corroborated; bytes not project-verified | Korean launch coverage; GameFAQs; GameTDB |
| WHITE2-HK | White 2 | Hong Kong | Japanese / TBD | 2012-06-23? | Unknown | Unknown | Unknown | Official territory support later confirmed; exact retail build unresolved | Nintendo Hong Kong; secondary release records |
| WHITE2-TW | White 2 | Taiwan | Japanese / TBD | 2012-06-23? | Unknown | Unknown | Unknown | Research target | Secondary release records; primary evidence pending |
| WHITE2-CA | White 2 | Canada | English/French packaging | 2012-10-07? | Unknown | `IRDO` family / exact retail suffix TBD | Unknown | Research target | Packaging/build evidence pending |
| WHITE2-NZ | White 2 | New Zealand | English / TBD | 2012-10-11? | Unknown | Unknown | Unknown | Research target | Primary/preservation evidence pending |
| WHITE2-SG | White 2 | Singapore / officially served Asian markets | English/Japanese / TBD | Unknown | Unknown | Unknown | Unknown | Research target | Primary/preservation evidence pending |

## Revision alert

Public preservation evidence requires special handling:

- No-Intro lists `IRDJ` revision 0 as undumped and notes a dumped `Rev 1` before release date.
- Other public catalogues index `Pocket Monsters - White 2 (Japan) (Rev 1)`.

Do not convert this into the claim "launch retail = Rev 1" until cartridge/header evidence and independent metadata are reconciled.

## Difference matrix

| Build ID | Category | Japanese baseline state | Regional state | Difference class | Evidence level | Source(s) | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| WHITE2-EU-FR / DE / IT / ES | language/build identity | Japanese `IRDJ` | Distinct language game codes (`IRDF`, `IRDD`, `IRDI`, `IRDS`) | text / localization / encoding; potentially other technical differences | Corroborated for product identity; technical diff pending | GameFAQs; GameTDB; preservation catalogues | Separate build targets must be retained independently. |
| WHITE2-KR | language/build identity | Japanese `IRDJ` | Korean `IRDK` | text / localization / encoding; fonts/glyphs; potentially other technical differences | Corroborated for product identity; technical diff pending | GameFAQs; GameTDB | Korean target is first-class, not a generic international variant. |
| WHITE2-US-EN / EU-EN / AU-EN | territory/build identity | Japanese `IRDJ` | Shared `IRDO` game-code family with different retail suffixes | unclassified until byte-comparison evidence exists | Corroborated for retail identity | Nintendo/secondary catalogues | Shared game code does not prove byte identity. |

## Difference classes

- executable / ARM9 / ARM7
- overlay
- filesystem / NitroFS
- NARC membership / ordering / format
- Pokémon / personal data / forms
- moves / abilities / items
- encounters
- trainers / AI / battle rules
- maps / matrices / warps / objects
- scripts / flags / variables / events
- text / localization / encoding
- fonts / glyphs
- graphics / sprites / UI / models
- audio / music / SFX
- save structure / checksums
- wireless / infrared / Wi-Fi
- C-Gear / Entralink / Game Sync / Global Link
- Mystery Gift / external distribution
- PWT / Pokéstar Studios / Join Avenue / Hidden Grotto / Medal / Memory Link / Key System / Funfest / White Treehollow
- unused / dummy / debug content
- bug / glitch / revision fix
- legal / ratings / censorship / localization adaptation
- packaging / manual / non-ROM material
- unclassified

## Evidence levels

- **Official** — official first-party material directly supports the claim.
- **Direct technical** — public code, extracted data, disassembly, or format implementation directly demonstrates the claim.
- **Corroborated** — two or more independent reliable sources agree.
- **Single-source** — one credible source exists but independent confirmation is pending.
- **Reported** — claim exists but technical verification is insufficient.
- **Unknown** — no adequate evidence yet.

## Source anchors

- https://www.nintendo.co.jp/ds/irej/index.html
- https://www.pokemon.co.jp/ex/b2w2/product/
- https://www.nintendo.co.jp/ir/pdf/2013/130131.pdf
- https://www.nintendo.com/en-gb/News/2012/Pokemon-Black-Version-2-Pokemon-White-Version-2-and-Pokemon-Dream-Radar-launching-October-12th-2012-647545.html
- https://gamefaqs.gamespot.com/ds/661226-pokemon-black-version-2/data
- https://wiki.no-intro.org/index.php?title=Nintendo_-_Nintendo_DS%28i%29_Japan_undumped
- https://www.gametdb.com/DS/IRDO
- https://www.gametdb.com/DS/IRDK

## Comparison rule

A localized text difference is not automatically a complete technical-ROM difference description. Record localization, then separately record any encoding, font, archive-layout, script, executable, or resource change.

A revision-specific bug fix must remain tied to the exact target until evidence shows it applies more broadly.
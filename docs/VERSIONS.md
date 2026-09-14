# Version Coverage

Use this document as the authoritative inventory of game versions targeted by this decompilation project.

The project has no local retail ROM baseline. Entries below therefore distinguish **release/product identity documented from public sources** from byte-level verification. A public catalogue hash or revision label is a research lead, not a project-level `Matched` result.

## Japanese baseline

| Status | Region / territory | Language | Revision / update | Product / build identifier | Release | Hashes | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Planned | Japan | Japanese | **Launch-retail revision unresolved.** Public preservation sources report a dumped `Rev 1` and list revision 0 as undumped. | `TWL-IRDJ-JPN` / game code `IRDJ` | 2012-06-23 | TBD | **Canonical survey baseline.** Nintendo/Pokémon official material confirms release date and product. Do not assume Rev 0 is the launch retail build; resolve cartridge revision evidence before assigning a baseline revision. |

## Regional / language targets

| Status | Region / territory | Language | Revision / update | Product / build identifier | Release | Hashes | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Planned | United States | English | TBD | `TWL-IRDO-USA` / `IRDO` | 2012-10-07 | TBD | North American launch date is independently documented; compare with EUR/AUS despite shared game code. |
| Planned | Australia | English | TBD | `TWL-IRDO-AUS` / `IRDO` | 2012-10-11 | TBD | Separate Australian retail identifier. |
| Planned | Europe | English | TBD | `TWL-IRDO-EUR` / `IRDO` | 2012-10-12 | Public reference: GameTDB CRC32 `b4416cec`, MD5 `51e380ed94bd5c70a9b46e3966f2cf88`, SHA-1 `a6c7e035063c6830d5ef7a28edf9152f1c3f59bf` | Nintendo Europe confirms 2012-10-12 launch. Public hash is not project-verified. |
| Planned | France / Europe | French | TBD | `TWL-IRDF-FRA` / `IRDF` | 2012-10-12 | TBD | Distinct French build identifier. |
| Planned | Germany / Europe | German | TBD | `TWL-IRDD-NOE` / `IRDD` | 2012-10-12 | Public reference: CRC32 `107b8669`, MD5 `40e4009ac3306dd18d04764d833a1595`, SHA-1 `4ed37674d2a09db4573bf579d2cc89c60794b59c` | Distinct German build identifier. |
| Planned | Italy / Europe | Italian | TBD | `TWL-IRDI-ITA` / `IRDI` | 2012-10-12 | TBD | Distinct Italian build identifier. |
| Planned | Spain / Europe | Spanish | TBD | `TWL-IRDS-ESP` / `IRDS` | 2012-10-12 | Public reference: CRC32 `44e04b67`, MD5 `5fdb174c0e2a4ab9305373b9e90d2664`, SHA-1 `bf65769c43cd4db26f88c76f7aeee201c9322f0e` | Distinct Spanish build identifier. |
| Planned | South Korea | Korean | Public catalogues report version 0; project verification pending | `TWL-IRDK-KOR` / `IRDK` | 2012-11-08 | Public reference: CRC32 `cf895342`, MD5 `4a7a098d122b24d04c2b2d6635db120f`, SHA-1 `57ce8d933ab593d05ce217b2a2e03e41979f5845` | Korean launch independently documented; hashes from GameTDB remain public-reference evidence only. |
| Planned | Hong Kong | Japanese / TBD | TBD | TBD | 2012-06-23? | TBD | Secondary sources report same-day availability and Nintendo Hong Kong later lists the title as supported. Exact retail SKU/build relationship to Japan must be established. |
| Planned | Taiwan | Japanese / TBD | TBD | TBD | 2012-06-23? | TBD | Secondary sources report same-day availability. Determine whether this was Japanese software distribution rather than a distinct executable build. |
| Planned | Canada | English/French packaging | TBD | likely `IRDO` family; exact retail suffix/build mapping TBD | 2012-10-07? | TBD | Dedicated packaging/build research required; do not collapse into US without evidence. |
| Planned | New Zealand | English / TBD | TBD | TBD | 2012-10-11? | TBD | Determine whether Australian build was distributed unchanged. |
| Planned | Singapore / other officially served Asian markets | English/Japanese / TBD | TBD | TBD | TBD | TBD | Research target; require primary or preservation evidence before defining a build. |

## Revision alert: Japanese White 2

Public preservation material creates a non-trivial revision question:

- No-Intro's Japan undumped list records `IRDJ` revision 0 as undumped and states that `Rev 1` was dumped before release date.
- GameHacking.org also indexes `Pocket Monsters - White 2 (Japan) (Rev 1)`.

This does **not** by itself prove every launch retail cartridge was Rev 1. The baseline remains `TBD` until cartridge/header evidence and independent preservation metadata are reconciled.

## Current source anchors

- Nintendo Japan B2W2 page: https://www.nintendo.co.jp/ds/irej/index.html
- Pokémon official B2W2 product page: https://www.pokemon.co.jp/ex/b2w2/product/
- Nintendo corporate regional release table: https://www.nintendo.co.jp/ir/pdf/2013/130131.pdf
- Nintendo Europe launch notice: https://www.nintendo.com/en-gb/News/2012/Pokemon-Black-Version-2-Pokemon-White-Version-2-and-Pokemon-Dream-Radar-launching-October-12th-2012-647545.html
- GameFAQs release/product catalogue: https://gamefaqs.gamespot.com/ds/661226-pokemon-black-version-2/data
- No-Intro Japan undumped research: https://wiki.no-intro.org/index.php?title=Nintendo_-_Nintendo_DS%28i%29_Japan_undumped
- GameTDB English entry: https://www.gametdb.com/DS/IRDO
- GameTDB Korean entry: https://www.gametdb.com/DS/IRDK

## Status vocabulary

- **Planned** — target is in scope; identity may be partly documented, but project-level build verification is not complete.
- **Verified** — exact target identity and hashes have been independently confirmed under the repository verification rules.
- **Mapped** — executable/data layout documented for that exact target.
- **In progress** — active source reconstruction.
- **Matched** — reconstruction verified against the exact target using a defined matching criterion.
- **Reference only** — used for comparison but not a reconstruction target.

## Recording rules

1. The Japanese release is the starting comparison baseline, but its exact revision must be proven rather than assumed.
2. Record exact revision/update information whenever known; use `TBD` when it is not.
3. Prefer cryptographic hashes over filenames as identity evidence, but distinguish public-reference hashes from project-verified hashes.
4. Do not commit retail game images, decrypted game images, console keys, or ROM binaries.
5. Record regional, territory, packaging, language, and revision differences instead of assuming releases are identical.
6. If two territories share a game code, byte identity still requires verification.
7. Link version-specific findings to relevant documentation, manifests, or verification records.
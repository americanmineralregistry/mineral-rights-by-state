# Mineral Rights Laws by State and Dormancy Risk Index, 2026 edition (United States)

A free, openly licensed dataset of U.S. mineral rights and dormant mineral laws for all 50 states and the District of Columbia, with a dormancy risk score for each jurisdiction. Maintained by American Mineral Registry.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20935347.svg)](https://doi.org/10.5281/zenodo.20935347)  License: CC BY 4.0

- Live, interactive version: https://americanmineralregistry.com/research/mineral-rights-by-state.html
- Permanent record and DOI: https://doi.org/10.5281/zenodo.20935347
- Maintained by: American Mineral Registry, https://americanmineralregistry.com

## What this is

A severed mineral interest can sit unused for decades. In some states an unused interest can lapse and revert to the surface owner, in others it never does, and the rules and deadlines vary widely. This dataset captures, for every U.S. state and D.C., whether an unused severed mineral interest can lapse, the mechanism and period where one exists, related provisions such as surface damages acts and forced pooling, and a 0 to 100 dormancy risk score. It is offered free under CC BY 4.0 so researchers, journalists, owners and developers can cite it directly.

## Headline figures (2026 edition)

Across 51 jurisdictions (50 states and the District of Columbia):

- 14 states where an unused severed mineral interest can lapse or revert to the surface owner.
- 6 states with a special preservation or reversion mechanism rather than a simple lapse.
- 31 jurisdictions, including the District of Columbia, where an unused severed interest does not lapse through nonuse.
- 11 states with a surface damages act.
- 34 states with forced or compulsory pooling.
- Highest dormancy risk: Louisiana, with a 10 years period (risk score 100 of 100).

Texas does not lapse a severed mineral interest through nonuse.

## Files

| File | What it is |
| --- | --- |
| `mineral-rights-by-state.csv` | The dataset, one row per jurisdiction, 14 columns. |
| `mineral-rights-by-state.json` | The same data as JSON, with a `meta` block and a `data` array. |
| `CITATION.cff` | Machine-readable citation metadata (GitHub reads this and shows a "Cite this repository" button). |
| `citation.bib` | BibTeX citation. |
| `citation.ris` | RIS citation, for reference managers. |

### Columns

- `state`, `abbr`: jurisdiction name and USPS abbreviation.
- `category`: lapse behavior class, one of `none`, `lapse`, `special`.
- `unused_minerals`: plain-language outcome for an unused interest (Does not lapse, Can lapse / revert, Special mechanism).
- `lapse_period`: the statutory dormancy period where one exists (for example 10 years, 20 years), else `none`.
- `surface_damages_act`: whether the state has a surface damages act (yes or no).
- `forced_pooling`: whether the state has forced or compulsory pooling (yes or no).
- `risk_score`: a 0 to 100 composite reflecting whether and how readily an unused severed interest can lapse.
- `rank`: 1 to 51 ranking by risk, where 1 is the highest risk.
- `statute`: statutory citation where applicable, else `n/a`.
- `source_status`: provenance flag (for example Sourced, or No dormant act (surveyed)).
- `source_url`: link to the primary source where available.
- `preservation`: short note on how an owner preserves the interest.
- `note`: longer plain-language explanation for the jurisdiction.

## How to cite

American Mineral Registry. (2026). Mineral Rights Laws by State and Dormancy Risk Index, 2026 edition (United States) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.20935347

Machine-readable citation metadata is in `CITATION.cff`, `citation.bib` and `citation.ris`.

## Methodology and caveats

The dataset is built from national statutory surveys and primary sources. Dormant mineral law is state-specific and changes over time, so the `note` field repeats a simple instruction: confirm against the current state code before relying on any single entry. This dataset is informational and is not legal advice.

## License

Creative Commons Attribution 4.0 International (CC BY 4.0). You may share and adapt the data, including commercially, with attribution.

Attribution string:
American Mineral Registry, Mineral Rights Laws by State and Dormancy Risk Index (2026), CC BY 4.0, https://doi.org/10.5281/zenodo.20935347

## About

American Mineral Registry publishes open data on U.S. mineral and royalty ownership. Site: https://americanmineralregistry.com

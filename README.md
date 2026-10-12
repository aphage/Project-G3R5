# From Grandparents to Grandees: Three Generations, Five Regions, and the Family Origins of the World's Billionaires

**三代到巨富：五区三代人生历程与超级富豪的家族出身**

A cross-national, three-generation life-course database of contemporary super-wealthy families, with an accompanying manuscript.

## About the study

This project constructs a **seven-role × nine-dimension × five-region** life-course database of contemporary billionaire families: **101 billionaire families (707 individuals)** spanning the United States, Europe, China, Japan, and South Korea. Each family is coded across **seven roles** (the billionaire, both parents, both paternal grandparents, and both maternal grandparents) and **nine life dimensions** (birth environment, basic education, higher education, family structure, marital status, occupational trajectory, industry, wealth trajectory, and major life events).

**Sample.** Families were identified from current and historical Forbes billionaire lists and selected purposively within each region for diversity (self-made and inheriting billionaires, industries, birth cohorts), not at random. Category shares therefore describe this sample, not the billionaire population.

The analysis is **exploratory and descriptive**. Five guiding expectations organize it; they took shape during data collection, so they are not treated as confirmatory hypotheses.

| Expectation | Question | Key evidence |
|---|---|---|
| H1 Family origin | Did most billionaires start from zero? | Among 82 with known origins: paternal ascent 41.5%, continuity 35.4%, low starting point 13.4% |
| H2 Era shock × family buffer | When did historical shocks interrupt schooling? | Born ≤1946: 8/12 from low-origin or ruined families vs. 0/22 from ascending or established families (Fisher p < 0.001); low-origin families born after 1946: 0/7 |
| H3 Inheritors' education | How does heirs' education differ from founders'? | Degree completion 92% (heirs) vs. 59% (founders from comfortable families), p = 0.010; university entry similar (96% vs. 89%) |
| H4 Record visibility | Who is recorded and remembered? | Name availability 100% (billionaire) → 2.0% (maternal grandmother); within-generation gender gaps up to 16.8 pp |
| H5 Cohort change | Did new industries lower old barriers? | Technical majors 59% vs. 37% (p = 0.056), but low starting points are rarer, not more common, among the young cohort (1/23 vs. 10/59) |

A conjecture that privacy is itself a resource of the wealthy ("active invisibility") is discussed as a direction for future research.

**A note on missingness.** Missing data are deliberately retained as data: under a common retrieval protocol, the distribution of availability reflects record-keeping structures, lineage, and gender inequality. Information was retrieved mainly through web search engines (AI-assisted), and a cell was coded missing when no qualifying source was found, so missingness also reflects online searchability; regional contrasts should be read with care. All missing cells are explicitly tagged "not documented"; nothing has been fabricated.

## Repository structure

```
G3R5-paper/
├── README.md
├── LICENSE
├── paper/
│   ├── PAPER_G3R5.tex                  # Manuscript (LaTeX, English)
│   ├── PAPER_G3R5.pdf                  # Compiled manuscript (18 pp)
│   ├── PAPER_G3R5_CN.tex               # Manuscript (LaTeX, Chinese; XeLaTeX)
│   ├── PAPER_G3R5_CN.pdf               # Compiled Chinese manuscript (15 pp)
│   ├── references.bib                  # BibTeX reference library (18 entries)
│   └── REVISION_NOTES_2026-10-12.md    # Changes made in the October 2026 revision
├── figures/
│   ├── fig1-history-and-family.png     # Interrupted schooling by birth cohort and family background
│   ├── fig2-who-gets-remembered.png    # Name availability across three generations
│   └── source/                         # HTML sources; render at 700 px wide, 2x scale
└── data/
    ├── all_people_v1.3_fixed.csv       # 707 individuals × 35 columns
    ├── all_events_v1.3_full.csv        # 733 life-course events
    ├── edu_path_v13.csv                # Education classification (C61/W15/D9/H7/U9)
    ├── h3_inheritors_recode_v14.csv    # Hand-coded education of the 28 inheritors
    ├── full_analysis_v1.3.json         # Machine-readable analysis (H1–H5, Kappa; corrected 2026-10-12)
    ├── CODING_SPEC.md                  # Coding scheme v1.3 (7 roles × 9 dimensions)
    ├── FIELD_DICTIONARY.md             # Field dictionary
    ├── DATA_README.md                  # Data documentation
    ├── HYPOTHESIS_VERIFICATION_v1.3.md # Original verification report (superseded in part; see errata at top)
    └── INTERCODER_RELIABILITY.md       # Coding consistency check (Cohen's Kappa = 0.628)
```

## Data quality

- **Coding consistency**: Cohen's Kappa = 0.628 (agreement 84%, n = 25, a 25% random sample of the education classification). First-pass codes were generated with an AI tool and reviewed by the author; the author then recoded the subsample from the raw texts without seeing the first-pass codes. Because the author was involved in both passes, this is a consistency check rather than independent intercoder reliability; an external recoding is planned. Four disagreements were adjudicated, two of them with additional source verification.
- **Reliability tags**: every data cell carries one of four tags (verified / single-source / inferred / missing).
- **Event causes**: every life-course event carries a cause grade (A self-statement / B authoritative record / C researcher inference / D unverifiable).

## Use of AI tools

Generative AI tools were used to retrieve and summarize public biographical information (including DataPro), for first-pass coding (reviewed by the author), for drafting, editing, and translating the manuscript, and for writing analysis code. Claude (Anthropic) was used to review the manuscript, verify references, and revise text and code. Every coded cell carries a source URL and reliability tag so it can be checked independently. See Section 4.5 of the manuscript.

## How to cite

```bibtex
@unpublished{g3r5,
  title  = {From Grandparents to Grandees: Three Generations, Five Regions,
            and the Family Origins of the World's Billionaires},
  author = {Ariia Xia},
  year   = {2026},
  note   = {Manuscript, available at https://github.com/aphage/Project-G3R5}
}
```

## License

All content in this repository (manuscript, data, and documentation) is licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0)**. See `LICENSE`.

## Status

Working paper / preprint stage. Submission to a peer-reviewed sociology journal (e.g., Socio-Economic Review, European Sociological Review, Research in Social Stratification and Mobility) is in preparation.

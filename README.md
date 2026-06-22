# The Relationship Between a Non-Western Migration Background and Education Level

**Authors:** Tamara Bakker, Rik de Bruijn, Joep Hagendoorn, Lize den Hertog, Isabelle Stankovski  
**Course:** Programming for Economists 2026 | Tutorial Group 2-1  
**Tutor:** Fatima Amankour

## Introduction

A study by research agency **SCALIQ** involving 6,409 secondary school students suggests that students with Arabic first and/or last names are more likely to be placed at a lower educational level than equally intelligent students with European-sounding names. About half of the students with Arabic names were placed approximately half a school level lower. The researchers indicate this may be a sign of inequality in education — a problem that can negatively affect students' educational trajectories, career opportunities, and motivation.

However, the SCALIQ study only examined intelligence scores and names, without accounting for other potentially relevant factors such as family income, home support, or cultural background.

A second study by **KIS (Kennisplatform Integratie & Samenleving)** investigated whether students with a migration background in the Netherlands receive lower educational recommendations than their abilities warrant. Based on quantitative analyses and interviews with teachers, students, and parents, the researchers found limited direct evidence of ethnicity-based discrimination. Nevertheless, factors such as Dutch language proficiency, home environment, classroom behavior, and teacher perceptions were found to potentially influence recommendations — and may disproportionately disadvantage children from non-Western backgrounds.

Together, these studies suggest that non-Western migrants in the Netherlands tend to attain lower levels of education than their Dutch peers. While establishing direct causal relationships is difficult, this educational gap represents a meaningful social problem: it contributes to income inequality, reinforces broader patterns of disadvantage, and limits opportunities for people with a migration background. Given the current political and public discourse around migration in the Netherlands, this issue is both timely and socially relevant.



## Datasets

This project uses three datasets:

| Dataset | Description | Source | Period |
|---|---|---|---|
| `Jaar_bevolking_migratie_achtergrond.csv` | Education level by migration background (age 15+) | CBS (2021) | 2003–2020 |
| `Ranglijst van de migratieachtergrond van inwoners per provincie in Nederland.xlsx` | Percentage of non-Western migrants per province | AlleCijfers (2026) | 2026 |
| `Regionale_kerncijfers_Nederland_04062026_120418.xlsx` | Education level participation per province | CBS (2025) | 2024 |



## Project Structure

```
PFE2026/
├── data/
│   ├── Jaar_bevolking_migratie_achtergrond.csv
│   ├── Ranglijst van de migratieachtergrond van inwoners per provincie in Nederland.xlsx
│   └── Regionale_kerncijfers_Nederland_04062026_120418.xlsx
├── analysis.Rmd        # Main R Markdown file with full analysis
└── README.md
```



## Key Findings

**Temporal trends (2003–2020)**  
People with non-Western migration backgrounds in the Netherlands have lower educational levels than those with Dutch backgrounds. Non-Western migrants make up a much larger share of people with only basic education, while university degrees (HBO/WO) are far more common among Dutch-born people. However, the gap has been narrowing over time, particularly at the bachelor level.

**Age group differences**  
The educational gap is largest among older age groups (75+: ~10% Dutch vs. ~3% non-Western hold a bachelor's degree), but becomes smaller for younger generations (25–35: ~32% Dutch vs. ~27% non-Western). This suggests younger people with non-Western backgrounds are increasingly obtaining higher education — yet a persistent gap of roughly 7 percentage points remains across most age groups.

**Policy impact: Wet inburgering (2006)**  
The share of non-Western migrants with only primary education as their highest level declined steeply after the introduction of the *Wet inburgering* in 2006. However, the trend levelled off at around 18–20%, suggesting the policy had a limited but not transformative effect.

**Regional variation**  
Non-Western migrants are concentrated primarily in Randstad provinces (Noord-Holland, Zuid-Holland, Utrecht). However, the educational gap exists across all provinces — including those with smaller non-Western populations — indicating that geographic concentration alone does not explain the inequality.

## Policy Implication

The findings suggest that investments in Dutch language support (tutoring and language programs) in primary and secondary schools may help reduce educational gaps, given that Dutch language proficiency is a key factor in academic success.

## How to Reproduce

1. Clone this repository:
   ```bash
   git clone https://github.com/RikdeBruijn/PFE2026
   ```
2. Open `analysis.Rmd` in RStudio.
3. Place all datasets in the `data/` folder.
4. Install required packages (listed at the top of the `.Rmd` file) and knit the document.

**Required R packages:** `tidyverse`, `readxl`, `cbsodataR`, `sf`, `rnaturalearth`, `rnaturalearthhires`, `gridExtra`, `patchwork`, `renv`



## References

- AlleCijfers (2026, June 8). *Ranglijst: autochtoon en migratieachtergrond van de bewoners per provincie in Nederland*. https://allecijfers.nl/ranglijst/autochtoon-en-migratieachtergrond-per-provincie-in-nederland/
- CBS (2025, November 7). *Bevolking; hoogstbehaald onderwijsniveau en regio*. https://opendata.cbs.nl/#/CBS/nl/dataset/85525NED/table
- CBS (2021, November 16). *Bevolking; onderwijsniveau en -richting 2003–2021*. https://opendata.cbs.nl/#/CBS/nl/dataset/82275NED/table
- Wet van 30 november 2006, houdende regels inzake inburgering in de Nederlandse samenleving (Wet inburgering). (2006). *Staatsblad van het Koninkrijk der Nederlanden*, No. 625. https://zoek.officielebekendmakingen.nl/stb-2006-625.pdf


## License

MITvan 30 november 2006, houdende regels inzake inburgering in de Nederlandse samenleving (Wet inburgering). (2006). *Staatsblad van het Koninkrijk der Nederlanden*, No. 625. https://zoek.officielebekendmakingen.nl/stb-2006-625.pdf

## License

MIT

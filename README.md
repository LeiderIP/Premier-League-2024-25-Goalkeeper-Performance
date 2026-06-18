# Premier League 2024/25 — Goalkeeper Performance

Post-Shot xG (PSxG) faced vs goals conceded for every regular goalkeeper in the 2024/25 Premier League season, built from StatsBomb event data.

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python) ![SVG](https://img.shields.io/badge/Viz-SVG%20%2B%20JS-orange?style=flat-square) ![Data](https://img.shields.io/badge/Data-StatsBomb-red?style=flat-square)

---

## Live Demo

**[Open Goalkeeper Performance](https://leiderip.github.io/Premier-League-2024-25-Goalkeeper-Performance/Goalkeeper_Performance.html)**

---

## Features

- **Season Overview** — scatter plot of PSxG faced vs goals conceded, one point per goalkeeper (min 900 minutes), sized by matches played, coloured by club. A diagonal reference line separates over- and under-performing shot-stoppers
- **Goalkeeper Detail** — search any keeper and see their full season shot-stopping map: every shot faced, plotted by location, coloured by outcome (saved/blocked vs goal), sized by how dangerous the chance was (PSxG)
- Stat cards: matches, minutes, save %, and Goals Prevented (PSxG faced minus actual goals conceded — the standard shot-stopping value metric)
- Hover any shot for the shooter's name, match, minute and PSxG
- **Dark / Light theme toggle**

---

## Method

**Post-Shot xG (PSxG)** estimates the probability a shot results in a goal based on where it was placed and how it was struck — unlike pre-shot xG, it accounts for the shot itself, making it the correct baseline for judging a goalkeeper's saves rather than the shooter's chance quality.

Goals Prevented = total PSxG faced − actual goals conceded. A positive value means the keeper conceded fewer goals than the shots they faced would suggest; negative means more.

**Own goals are excluded** from goals conceded, since there is no shot event or PSxG value for the goalkeeper to be evaluated against — the standard convention in goalkeeper analytics.

Only goalkeepers with at least 900 minutes (≈10 full matches) are included, filtering out emergency or one-off appearances by outfield players or third-choice keepers.

---

## Portfolio

| Project | Link |
|---|---|
| Title Race | [Live](https://leiderip.github.io/Premier-League-2024-25-Title-race/pl_position_race.html) |
| xG Race Explorer | [Live](https://leiderip.github.io/Premier-League-2024-25-xG-Title-race-/xG_Race_Explorer.html) |
| Season Shot Map | [Live](https://leiderip.github.io/Premier-League-2024-25-Shot-Map/Shot_Map.html) |
| Top Scorers vs xG | [Live](https://leiderip.github.io/Premier-League-2024-25-Top-Scorers-xG/Top_Scorers_xG.html) |
| Player Heatmap | [Live](https://leiderip.github.io/Premier-League-2024-25-Player-Heatmap/Player_Heatmap.html) |
| Scouting Radar | [Live](https://leiderip.github.io/Premier-League-2024-25-Scouting_Radar/Scouting_Radar.html) |
| Pass Network | [Live](https://leiderip.github.io/Premier-League-2024-25-Pass-Network/Pass_Network.html) |
| Match Momentum | [Live](https://leiderip.github.io/Premier-League-2024-25-Match-Momentum/Match_Momentum.html) |
| Goalkeeper Performance | This project |

---

*Data © StatsBomb.*

# 2026 NFL Team and Bye-Week Reference

> **Purpose:** Fast normalization and bye-week lookup for the HAL 9000s live draft copilot.  
> **Bye-week status:** **Confirmed for all 32 teams** from the NFL's official 2026 schedule release. The NFL states that 2026 byes run from Week 5 through Week 14, with no byes in Week 12.

## Primary Lookup Table

| ESPN | Team | Conf | Division | 2026 Bye | Normalize aliases |
|---|---|---|---|---:|---|
| ARI | Arizona Cardinals | NFC | West | 14 | ARZ |
| ATL | Atlanta Falcons | NFC | South | 11 | — |
| BAL | Baltimore Ravens | AFC | North | 13 | — |
| BUF | Buffalo Bills | AFC | East | 7 | — |
| CAR | Carolina Panthers | NFC | South | 5 | — |
| CHI | Chicago Bears | NFC | North | 10 | — |
| CIN | Cincinnati Bengals | AFC | North | 6 | — |
| CLE | Cleveland Browns | AFC | North | 11 | — |
| DAL | Dallas Cowboys | NFC | East | 14 | — |
| DEN | Denver Broncos | AFC | West | 10 | — |
| DET | Detroit Lions | NFC | North | 6 | — |
| GB | Green Bay Packers | NFC | North | 11 | GNB |
| HOU | Houston Texans | AFC | South | 8 | — |
| IND | Indianapolis Colts | AFC | South | 13 | — |
| JAX | Jacksonville Jaguars | AFC | South | 7 | JAC |
| KC | Kansas City Chiefs | AFC | West | 5 | KAN |
| LV | Las Vegas Raiders | AFC | West | 13 | OAK |
| LAC | Los Angeles Chargers | AFC | West | 7 | SD, SDG |
| LAR | Los Angeles Rams | NFC | West | 11 | STL |
| MIA | Miami Dolphins | AFC | East | 6 | — |
| MIN | Minnesota Vikings | NFC | North | 6 | — |
| NE | New England Patriots | AFC | East | 11 | NWE |
| NO | New Orleans Saints | NFC | South | 8 | NOR |
| NYG | New York Giants | NFC | East | 8 | — |
| NYJ | New York Jets | AFC | East | 13 | — |
| PHI | Philadelphia Eagles | NFC | East | 10 | — |
| PIT | Pittsburgh Steelers | AFC | North | 9 | — |
| SF | San Francisco 49ers | NFC | West | 8 | SFO |
| SEA | Seattle Seahawks | NFC | West | 11 | — |
| TB | Tampa Bay Buccaneers | NFC | South | 10 | TAM |
| TEN | Tennessee Titans | AFC | South | 9 | — |
| WSH | Washington Commanders | NFC | East | 7 | WAS |

### Abbreviation Policy

- The **ESPN** column is the canonical key to use when parsing ESPN draft data.
- ESPN's current 2026 team shorthand is corroborated by ESPN's own all-team 2026 coverage, which uses: `ARI ATL BAL BUF CAR CHI CIN CLE DAL DEN DET GB HOU IND JAX KC LAC LAR LV MIA MIN NE NO NYG NYJ PHI PIT SF SEA TB TEN WSH`.
- `Normalize aliases` are compatibility aliases for external feeds, historical data, or common alternate shorthand. They are **not claims that ESPN currently emits those aliases**.
- For relocated franchises, map historical city abbreviations to the current franchise only when the data clearly refers to the NFL team/franchise (for example `OAK -> LV`, `SD -> LAC`, `STL -> LAR`).

## 2026 Bye Weeks by Week

- **Week 5:** CAR, KC
- **Week 6:** CIN, DET, MIA, MIN
- **Week 7:** BUF, JAX, LAC, WSH
- **Week 8:** HOU, NO, NYG, SF
- **Week 9:** PIT, TEN
- **Week 10:** CHI, DEN, PHI, TB
- **Week 11:** ATL, CLE, GB, LAR, NE, SEA
- **Week 12:** none
- **Week 13:** BAL, IND, LV, NYJ
- **Week 14:** ARI, DAL

The NFL specifically identifies **Week 11 as the only six-team bye week**, making it the largest single-week concentration risk in 2026.

## How the Live Draft Copilot Should Use Bye Weeks

1. Resolve each drafted player's bye from the player's NFL team using the table above.
2. Track bye concentration across the HAL 9000s roster, especially among likely weekly starters.
3. Track opponent bye concentrations as contextual evidence when predicting what teams between HAL 9000s picks may do.
4. Use bye pressure as a **tiebreaker/contextual factor**, not as a reason to pass on materially superior player value.
5. Distinguish:
   - **starter collision:** multiple likely starters unavailable together;
   - **bench collision:** usually low concern;
   - **opponent pressure:** an opponent may prefer a different player if the top option compounds a severe bye problem.
6. Never infer a player's bye from position or draft rank. Resolve it from the player's NFL-team key.

## Verification Sources

**Official NFL source — confirmed 2026 bye weeks:**  
NFL.com, “2026 NFL schedule release: Every team's bye week,” published May 15, 2026.  
https://www.nfl.com/news/2026-nfl-schedule-release-every-team-bye-week

**Official NFL schedule pages — corroboration:**  
https://www.nfl.com/schedules/2026/

**ESPN abbreviation corroboration:**  
ESPN's 2026 all-team draft coverage uses the canonical shorthand listed above.  
https://www.espn.com/nfl/draft2026/

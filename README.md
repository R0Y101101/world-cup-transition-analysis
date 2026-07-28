# 2022 World Cup Transition Speed Analysis

## Overview

This project analyzes how quickly teams progressed the ball after regaining
possession during the 2022 FIFA World Cup.

The main research question was:

> After winning possession in open play, how does forward progression rate
> affect shot creation and expected goals, and does the answer depend on
> where the ball is won?

## Data

- Source: StatsBomb Open Data
- Competition: 2022 FIFA World Cup
- Matches analyzed: 64
- Recorded events: 234,637
- Valid transitions analyzed: 2,074

An open-play regain was identified using ball recoveries, interceptions,
duels, and blocks that resulted in possession.

## Method

For each possession:

1. Identify where possession was regained.
2. Follow the possession for up to 15 seconds.
3. Measure forward progression.
4. Calculate progression speed as forward distance divided by time.
5. Classify transitions as slow, medium, or fast within each starting third.
6. Measure whether a shot occurred and the total expected goals generated.

## Main Findings

- Fast attacking-third transitions produced a 39.5% shot rate.
- Fast midfield transitions produced shots about 8.5 times as often as slow
  midfield transitions.
- Fast attacking-third transitions generated approximately 10 times the
  average xG of slow transitions.
- In the defensive third, maximum speed was not always the strongest option.

## Coaching Takeaway

> Win it high, sprint it forward. Win it deep, keep your head.

Teams should attack quickly after higher recoveries, while deeper recoveries
may benefit from a more controlled buildup.

## Repository Contents

- `analysis/`: R scripts used for data processing and analysis
- `graphs/`: Final charts produced in R
- `presentation/`: Final presentation
- `data/`: Data source and access information

## Tools

- R
- tidyverse
- ggplot2
- StatsBomb Open Data

## Author

Roy Nunez  
Wharton Moneyball Academy, 2026

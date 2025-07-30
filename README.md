# MLB Player Analysis System

A comprehensive Python-based analysis tool for exploring and analyzing Major League Baseball batting statistics from 2016-2025. This system provides detailed player analytics, comparisons, team analysis, and league-wide trend analysis with interactive visualizations.

## Features

### Player Analysis
- **Player Search & Overview**: Search for players and get comprehensive career statistics
- **Performance Trends**: Analyze player performance over time with detailed visualizations
- **Advanced Metrics**: Deep dive into power metrics, plate discipline, consistency, and baserunning
- **Career Patterns**: Analyze career development and identify peak performance periods
- **Rankings & Percentiles**: See how players rank among their peers with percentile rankings

### Comparison Tools
- **Head-to-Head Player Comparisons**: Compare two players across multiple statistical categories
- **Visual Comparisons**: Side-by-side performance charts and timeline analysis
- **Normalization**: Compare players from different eras with normalized metrics

### Team & League Analysis
- **Team Performance**: Analyze team batting statistics by season
- **Position Analysis**: Compare performance across different fielding positions
- **Season Leaders**: Find league leaders in specific statistical categories
- **League Trends**: Track how the game has evolved over time with trend analysis

### One-Click Analysis
- **Complete Player Reports**: Generate comprehensive analysis reports with a single function call
- **Interactive Visualizations**: Dynamic charts showing trends, comparisons, and distributions
- **Statistical Insights**: Automated insights and performance ratings

## Data Overview

The system analyzes **1,550+ player seasons** covering:
- **Seasons**: 2016-2025
- **Players**: 500+ unique MLB players
- **Teams**: All 30 MLB franchises
- **Statistics**: 35+ batting metrics including advanced sabermetrics

### Key Metrics Included
- Traditional stats: AVG, HR, RBI, SB, etc.
- Advanced metrics: WAR, OPS+, ISO, wRC+
- Plate discipline: BB%, K%, BB/K ratio
- Sabermetrics: rOBA, Rbat+, Total Bases

## Quick Start

### Prerequisites
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### Basic Usage

```python
# Load the system
exec(open('MLBPlayerAnalysisBatting2016-2025.ipynb').read())

# Search for a player
search_players('Judge')

# Complete analysis for a player
quick_player_analysis('Aaron Judge')

# Compare two players
compare_players('Aaron Judge', 'Shohei Ohtani')

# Analyze team performance
analyze_team_batting('NYY', 2024)

# Find season leaders
season_leaders(season=2024, category='home_runs')
```

## Available Functions

### Player Analysis Functions
| Function | Description |
|----------|-------------|
| `search_players(name)` | Search for players by name pattern |
| `get_player_overview(player)` | Comprehensive player overview |
| `analyze_player_trends(player)` | Performance trends with visualizations |
| `get_player_rankings(player, season)` | Player rankings and percentiles |
| `advanced_player_analysis(player)` | Deep statistical analysis |
| `quick_player_analysis(player)` | Complete one-click analysis |
| `analyze_career_path(player)` | Career development patterns |

### Comparison Functions
| Function | Description |
|----------|-------------|
| `compare_players(player1, player2)` | Head-to-head player comparison |

### Team & League Functions
| Function | Description |
|----------|-------------|
| `analyze_team_batting(team, season)` | Team batting analysis |
| `position_analysis(position, season)` | Performance by position |
| `season_leaders(season, category)` | Find statistical leaders |
| `analyze_league_trends(start, end)` | League-wide trend analysis |

## Example Analyses

### Player Overview
```python
get_player_overview('Ronald Acuña Jr.')
```
**Output**: Career totals, averages, season-by-season stats, best season, awards

### Performance Trends
```python
analyze_player_trends('Juan Soto')
```
**Output**: Multi-panel charts showing batting average, OBP/SLG, home runs, and WAR trends

### Advanced Analysis
```python
advanced_player_analysis('Mike Trout')
```
**Output**: Power metrics, plate discipline, consistency analysis, baserunning, age curves

### Player Comparison
```python
compare_players('Mookie Betts', 'Ronald Acuña Jr.')
```
**Output**: Side-by-side career totals, averages, normalized comparison charts, head-to-head timelines

## Data Structure

The system uses `batting_all_seasons.csv` with the following key columns:

**Basic Info**: `player_name`, `Season`, `age`, `team`, `position`
**Counting Stats**: `games`, `at_bats`, `hits`, `home_runs`, `runs_batted_in`, `stolen_bases`
**Rate Stats**: `batting_average`, `on_base_percentage`, `slugging_percentage`, `on_base_plus_slugging`
**Advanced**: `WAR`, `ops_plus`, `rOBA`, `Rbat+`, `total_bases`
**Other**: `Awards`, `strikeouts`, `walks`, `doubles`, `triples`

## Key Insights

The system automatically provides insights such as:
- **Player Ratings**: Elite, All-Star, Very Good, Above Average, Average, Below Average
- **Trend Analysis**: Improving, declining, or consistent performance patterns
- **Peak Identification**: Best seasons and career prime years
- **Consistency Metrics**: Performance variability analysis
- **Position Context**: How players compare within their position
- **League Context**: Performance relative to league averages

## Use Cases

### For Analysts
- Player evaluation and scouting
- Performance trend identification
- Contract and trade analysis
- Historical comparisons

### For Fans
- Settle debates between favorite players
- Understand player development
- Track team performance
- Explore baseball history

### For Researchers
- Analyze league trends
- Study positional differences
- Examine career patterns
- Generate statistical insights



## System Features

- **Error Handling**: Graceful handling of missing players/data
- **Data Validation**: Automatic data quality checks
- **Flexible Filtering**: Season-specific or career-wide analysis
- **Rich Visualizations**: Professional-quality charts and graphs
- **Performance Optimization**: Efficient data processing for large datasets
- **Extensible Design**: Easy to add new analysis functions

## Notes

- All statistics are for batting performance only
- Data includes both AL and NL players
- Advanced metrics calculated using standard sabermetric formulas
- Minimum plate appearance thresholds applied for rate statistics
- Awards data includes MVP, All-Star, Gold Glove, Silver Slugger, and Rookie of the Year

## Sample Output

```
PLAYER OVERVIEW: Aaron Judge
============================================================
Seasons Played: 5 seasons (2017, 2018, 2021, 2022, 2024)
Teams: NYY
Position: 9/DH
Age Range: 25-32

CAREER TOTALS:
   Games: 730
   At Bats: 2633
   Hits: 784
   Home Runs: 238
   RBIs: 554
   Walks: 522
   WAR/Season: 8.32

BEST SEASON: 2022
   Slash Line: .311/.425/.686
   62 HR, 131 RBI, 133 Runs
   WAR: 11.4
```

---

**Built for baseball analytics enthusiasts, by baseball analytics enthusiasts**

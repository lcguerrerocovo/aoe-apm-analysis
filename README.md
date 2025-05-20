# AOE2 APM Analysis

This repository contains a Jupyter notebook for analyzing Actions Per Minute (APM) in Age of Empires 2 replay files.

## Features

- Parse AOE2 replay files (.aoe2record)
- Extract player actions and timestamps
- Calculate APM (Actions Per Minute) for each player
- Visualize action distribution over time
- Compare different action types in stacked bar charts

## Setup

### Prerequisites

- Python 3.8+
- pip

### Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/aoe-apm-analysis.git
cd aoe-apm-analysis
```

2. Create a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Running the notebook

Launch Jupyter notebook:
```bash
jupyter notebook
```

Then open `apm_analysis.ipynb` in your browser.

## Usage

The notebook can process AOE2 replay files (.aoe2record) and generate visualizations of player actions.

1. Place your replay files in the project root directory
2. Follow the examples in the notebook to analyze your own replay files
3. Customize the analysis by modifying the action types to include/exclude

## Action Types Reference
Below is a list of common action types found in Age of Empires II replay files, including Definitive Edition (DE) actions. Each action type represents a specific command or event in the game.

| Action Type | Description |
|---------------------|-----------------------------------------------------------------------------|
| ATTACK | Orders unit(s) to attack a target. |
| STOP | Stops the current action of unit(s). |
| AI_PRIMARY | AI primary action. |
| MOVE | Orders unit(s) to move to a location. |
| AI_MOVE | AI move action. |
| RESIGN | Player resigns from the game. |
| WAYPOINT | Sets a waypoint for unit(s). |
| STANCE | Changes the stance (aggressive, defensive, etc.) of unit(s). |
| GUARD | Orders unit(s) to guard another unit. |
| FOLLOW | Orders unit(s) to follow another unit. |
| PATROL | Orders unit(s) to patrol between points. |
| FORMATION | Sets the formation for selected unit(s). |
| SAVE & EXIT | Saves and exits the game. |
| AI_COORD | AI coordinate action. |
| AI_TRAIN | AI trains a unit. |
| TECH | Researches a technology. |
| BUILD | Orders unit(s) to build a structure. |
| MULTIPURPOSE | Multipurpose action (context-dependent). |
| WALL | Orders unit(s) to build a wall. |
| DELETE | Deletes a unit or building. |
| ATTACKGROUND | Orders unit(s) to attack a ground location. |
| TRIBUTE | Sends resources to another player. |
| REPAIR | Orders unit(s) to repair a unit/building. |
| UNGARRISON | Ungarrisons unit(s) from a building. |
| GATE | Orders unit(s) to build a gate. |
| FLARE | Sends a flare on the map. |
| GARRISON | Garrison unit(s) in a building. |
| TRAIN | Trains a unit at a building. |
| RALLY | Sets a rally point for a building. |
| SELL | Sells resources at the market. |
| BUY | Buys resources at the market. |
| RELIC | Relic-related action. |
| TOWNBELL | Rings the town bell (garrison villagers). |
| BACKTOWORK | Sends villagers back to work after a town bell. |
| GAMESTATS | Game statistics event. |
| DE_ATTACK_MOVE | DE only: Orders unit(s) to attack-move (move and attack along the way). |
| DE_QUEUE | DE only: Queue-related action (e.g., multi-queue). |
| DE_MULTI_GATHERPOINT| DE only: Sets multiple gather points. |
| DE_TRANSFORM | DE only: Unit transformation (e.g., upgrades, morphs). |
| DE_GARRISON | DE only: Garrison action in DE. |
| DE_UNGARRISON | DE only: Ungarrison action in DE. |
| DE_FORMATION | DE only: Formation change in DE. |

> For a full and up-to-date list, see the [mgx-format](https://github.com/stefan-kolb/aoc-mgx-format/tree/master/spec/body/actions) spec

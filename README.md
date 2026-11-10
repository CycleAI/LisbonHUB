# LisbonHUB · safety mapping and route planning

Code and data for the VoxPop Lisbon project and the study **Data-Driven Approach
for Urban Micromobility Enhancement through Safety Mapping and Intelligent Route Planning**.

## Repository version

This is the earlier standalone CycleAI snapshot of the VoxPop Lisbon work.
For the collaboration fork, see [CycleAI/Lisbon-Hub](https://github.com/CycleAI/Lisbon-Hub),
which retains its connection to [VoxPop-Open-Call/Lisbon-Hub](https://github.com/VoxPop-Open-Call/Lisbon-Hub).

Both CycleAI repositories contain the same four analysis notebooks and matching
route-data values. The different bytes in `routing_results.csv` come from line
endings, not different observations. Use the collaboration fork as the starting
point for this project; the standalone repository preserves its separate history.
Record the repository and commit when reproducing an analysis.

## Explore the project

| Location | Contents |
| --- | --- |
| [src/](src/) | Random-point generation, route checking, route-factor calculation and Google distance comparison notebooks. |
| [data/](data/README.md) | Route outputs, filtered analyses and the 100-route comparison tables. |
| [routeExample/](routeExample/) | Shortest, balanced and safest route examples, plus a GeoJSON benchmark. |
| [img/](img/) | Heatmaps of detected streetscape features. |

## Notebook guide

| Notebook | Purpose |
| --- | --- |
| [Generate random points](src/20230525_OneHundredRandomPoints_CycleAI.ipynb) | Generate 100 points within the study boundary using geographic data. |
| [Check route results](src/20230607_RouteResultsChecker.ipynb) | Check route types, coordinates, distances and durations. |
| [Calculate route factors](src/routeFactorCalculator.ipynb) | Compare the shortest, balanced and safest route alternatives. |
| [Google distance comparison](src/googleDistanceCalculator.ipynb) | Obtain distance and duration comparisons through the Google Maps API. |

Read the notebook's imports and input/output paths before running it. Supply your
own API access where required. A fully pinned environment and one-command rebuild
are not provided. Use the [data guide](data/README.md) to distinguish intermediate
route outputs from the curated comparison tables.

## Attribution and reuse

The original notebook documentation credits [Tiago Tamagusko](https://github.com/tamagusko)
and dates the work to May–June 2023. Keep that attribution when reusing the work.
Check upstream project and data-source terms; public availability alone does not
establish permission to redistribute all inputs.

[CycleAI research catalogue](https://github.com/CycleAI) · [Contact](mailto:contact@cycleai.net)

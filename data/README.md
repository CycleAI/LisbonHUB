# About this data

This data folder is part of the VoxPop Lisbon project by CycleAI. It contains multiple CSV files used in the data analysis and route generation process.

## Data Files

### 1. routing_results.csv

This file contains the routing results produced by our system for all routes.

### 2. routes_without_errors.csv

This file contains all the routes without any detected errors. It was generated but not used in our final analysis. We opted to use the filtered_data.csv file instead.

### 3. routes_checked.csv

This file contains all routes that were checked by our team. It was used to deploy preliminary results.

### 4. filtered_data.csv

This file contains all data where no routing or consistency errors were detected. It is a curated subset of the overall data, selected for further analysis.

### 5. 100routesResult.csv

This file contains 100 routes selected at random from the eligible ones, filtered from the overall data.

### 6. 100routesResultGoogle.csv

This file contains the routing results produced by Google Maps for comparison. The routes are the same as those found in the 100routesResult.csv file.

### 7. 100routesResultComplete.csv

This file contains the final set of 100 routes, with both our calculated routes and those calculated by Google Maps. It provides a comprehensive overview of the routes, allowing for direct comparison between our routing system and Google Maps.

---

For any questions or feedback about the data files, please contact the author at <contact@cycleai.net>.

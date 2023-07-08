# LisbonHUB: Advancing Urban Micromobility

## A Data-Driven Approach to Safety Mapping and Intelligent Route Planning in Lisbon

This repository is part of the VoxPop Lisbon project by CycleAI.

## Overview

This repository contains a collection of Jupyter notebooks that serve two primary functions - to generate a set of random points and to validate and calculate a route factor for each route (shortest, balanced, safest) based on those points.

## Notebooks

### 1. One Hundred Random Points Generator

**Author:** Tiago Tamagusko (<tamagusko@gmail.com>)  
**Version:** 0.1 beta  
**Date:** 2023-05-25  

This notebook creates 100 random points within set limits.

Data Source: [Nominatim API](https://nominatim.openstreetmap.org/search.php?q=Lisbon+Portugal&polygon_geojson=1&format=json)  

### 2. Route Factor Calculator

**Author:** Tiago Tamagusko (<tamagusko@gmail.com>)  
**Version:** 0.1 beta  
**Date:** 2023-06-22  

This notebook calculates a route factor for each type of route (shortest, balanced, safest) using the following formula:

$$
\text{Route factor} = \frac{1}{k} \times \left(\sum_{i=1}^k\frac{\text{0,6} \times \text{TravelTime}}{ \text{15 min}} + \sum_{i=1}^k\frac{\text{0,4} \times \text{TotalDistance}}{\text{5 km}}\right)
$$

where:

- $k$ is the number of elements in each route type.
- $\text{TravelTime}$ is the travel time for each route, measured in minutes.
- $\text{TotalDistance}$ is the total distance for each route, measured in kilometers.

### 3. Route Results Checker

**Author:** Tiago Tamagusko (<tamagusko@gmail.com>)  
**Version:** 0.1 beta  
**Date:** 2023-06-07  

This notebook validates the output results of the routes. It checks the consistency of calculated paths, correct route types, consistent coordinates, distances, and durations. The results of these tests are recorded in the 'test_code' column in the dataset with specific codes assigned to each type of error.

## Error Codes

0: No errors detected.  
1: Not all routes were calculated.  
2: Error in path calculation (route_type not correctly classified as 'safe', 'balanced' or 'shortest').  
3: Inconsistent coordinates for source or destination on different routes for the same route_id.  
4: Inconsistent distances (shortest distance greater than balanced, or balanced distance greater than safest).  
5: Inconsistent durations (shorter duration longer than balanced, or balanced duration longer than safest).  

---

For any questions or feedback, please contact the author at <contact@cycleai.net>.

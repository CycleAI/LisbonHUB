I would suggest updating your README to look something like this:

"# LisbonHUB: Advancing Urban Micromobility

## A Data-Driven Approach to Safety Mapping and Intelligent Route Planning

This repository is part of the VoxPop Lisbon project by CycleAI.

## Overview

This repository contains the codes and data to be able to reproduce the article "Data-Driven Approach for Urban Micromobility Enhancement through Safety Mapping and Intelligent Route Planning".

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

This notebook calculates a route factor for each type of route (shortest, balanced, safest) using a specific formula.

### 3. Route Results Checker

**Author:** Tiago Tamagusko (<tamagusko@gmail.com>)  
**Version:** 0.1 beta  
**Date:** 2023-06-07  

This notebook validates the output results of the routes. It checks the consistency of calculated paths, correct route types, consistent coordinates, distances, and durations.

### 4. Google Maps Distance and Duration Calculator

**Author:** Tiago Tamagusko (<tamagusko@gmail.com>)  
**Version:** 0.1 beta  
**Date:** 2023-06-23  

This Python script calculates the distance and travel time between two sets of coordinates using the Google Maps Distance Matrix API. The data is read from a CSV file, the calculations are performed, and the results are written back into the dataset.

---

For any questions or feedback, please contact the author at <contact@cycleai.net>."

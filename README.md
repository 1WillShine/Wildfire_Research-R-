# Quantifying Wildfire Drivers in California Using Fire Weather Index Data
# -California Wildfire Risk Analysis Using Fire Weather Index (FWI)-

This project investigates the key environmental and meteorological factors driving wildfire activity and spread in California. Using Fire Weather Index (FWI) data and R-based statistical analysis, this study identifies which variables most strongly influence wildfire frequency and burned area during peak fire seasons.

## Overview

Wildfires pose a major environmental and economic threat in California. This project analyzes FWI variables—including moisture codes, spread indices, and weather conditions—to determine which factors show the strongest association with wildfire severity. The analysis emphasizes seasonal trends, focusing on August and September, the months with the highest observed wildfire activity.

## Dataset

The analysis uses the "Forest Fires" dataset compiled by Paulo Cortez and Aníbal Morais (University of Minho, 2007).  
Key properties:

- 517 records  
- 13 variables (12 predictors, 1 target)  
- No missing values  
- Includes temperature, humidity, wind, rainfall, spatial coordinates, and FWI moisture/spread indices  
- Target variable: burned area (hectares)

### Variables

- Spatial: X, Y  
- Temporal: month, day  
- Weather: temperature, relative humidity (RH), wind, rain  
- FWI moisture codes: FFMC, DMC, DC  
- FWI behavior indices: ISI  
- Target: burned area  

## Methodology

### 1. Seasonal Trend Analysis

- Grouped wildfire occurrences and burned area by month.
- Identified seasonal spikes using bar plots created in ggplot2.
- Found pronounced peaks in August and September.

### 2. Percentage Increase Calculations

To determine which FWI variables showed the greatest seasonal change:

- Calculated mean values for each variable during August and September.
- Compared them against the overall dataset mean.
- Computed percentage increases separately for each variable and again combined across the two peak months.
- Visualized results using bar charts in ggplot2.

### 3. Focus Variables

The analysis focused on:

- FFMC (Fine Fuel Moisture Code)  
- DMC (Duff Moisture Code)  
- DC (Drought Code)  
- ISI (Initial Spread Index)  
- Temperature  
- Relative humidity  
- Wind speed  

These variables represent fuel moisture, deep-soil drought, and fire spread conditions.

## Results

### Seasonal Trends
- Wildfire occurrences and burned area peak sharply in **August** and **September**.
- Visualizations confirm these as the months of highest fire activity.

### Key Drivers
- **DMC (Duff Moisture Code)**  
- **DC (Drought Code)**  

These two variables show the **largest percentage increases** during peak wildfire months.

### Interpretation
- DMC measures moisture in deep organic soil layers; higher values mean drier material that ignites more easily.
- DC reflects long-term drought conditions, strongly tied to climate change and land-use patterns.
- Together, these variables help explain elevated wildfire spread and intensity during peak season.

## Conclusion

The analysis demonstrates that DMC and DC are the primary environmental drivers associated with increased wildfire severity in California. Monitoring these variables—especially leading into August and September—may improve early-warning systems and resource planning for wildfire management. Future work could incorporate predictive modeling or integrate additional climate variables to expand the analytical framework.

## Repository Structure

You may organize this repository as follows:




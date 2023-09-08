# Earthquake Dashboard
<img src = "https://github.com/chanronnie/Tableau/blob/main/earthquake/image/DSI%20Earthquake%20Logo.png" width="800">

This folder contains the dataset I used to build my Tableau dashboard, which helps me sharpen my data visualization skills with Tableau. 

## Tableau of Contents
* [About Data](about-data)
* [Tableau Concepts](#tableau-concepts)
* [Dashboard Requirements](#dashboard-requirements)
* [Earthquake Dashboard](#earthquake-dashboard)
* [Copyright](#copyright)

## About Data
The dataset I used to create my Tableau dashboard is available for download in the description box of Andrew Jones' tutorial video. It contains records of earthquakes that occurred from July 2022 to August 10th, 2020, spanning 30 days. This dataset includes information such as the intensity of the earthquakes in terms of `magnitude`, the location (`longitude` and `latitude`) of the earthquakes, and the `date and time` of each incident.

- View dataset: [earthquake-data.csv](https://github.com/chanronnie/Tableau/blob/main/earthquake/earthquake-data.csv)
- Source: [here](https://www.youtube.com/watch?v=rf7sxW4iVAs&list=PLsmRQcJN_xK7qSqillLkHPDdH0_uM0jFx&index=2)


## Tableau Concepts

- Filters
- Pages (DateTime/Location as video)
- Calculated Field 

    - **`Counter`** : Count the number of records by simply writing "1" in the code
    - **`Max Value Fixed`**: Use with level of detail expression to lock in the maximum value for all records
    - **`Ratio`**: calculations

- Level of Detail (LOD): `{TYPE [Dimension List]: Aggregation}`</br> ex: `{FIXED: MAX([Magnitude])}`
</br> ex: `{FIXED [Location-Broad] : MAX([Magnitude])}` (see this as finding a max value using `group by` statement)

## Dashboard Requirements
### Features
1. A map showing where earthquakes took place, and its intensity in terms of magnitude
2. A list of the top 10 biggest earthquakes so we can easily isolate those
3. A breakdown of the percentage of earthquakes that occurred in each broad location
4. For each of the more granular location, show 
    - how many earthquakes took place
    - what the average magnitude was, and 
    - what the maximum magnitude was
### Final Dashboard
All these requirements must be attached to a single date filter, where we can track earthquakes day by day, with the ability to manually scroll through one day at a time and have everything we update as we do.

## Earthquake Dashboard
<img src = "https://github.com/chanronnie/Tableau/blob/main/earthquake/image/tableau_earthquake.png" width="800">

Access my dashboard on Tableau Public: [here](https://public.tableau.com/views/DSEarthquakeTracker/DSEarthquakeTracker?:language=en-US&:display_count=n&:origin=viz_share_link)

## Copyright
This is a project guided by [Andrew Jones (Data Science Infinity)](https://www.youtube.com/@andrew-jones-data-science) with some personalized modifications.

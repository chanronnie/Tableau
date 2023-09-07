# Earthquake Dashboard


## Concepts

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

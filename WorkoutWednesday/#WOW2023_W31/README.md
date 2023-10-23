# WOW2023 WEEK 31 - Can you find the most popular sub-category by sales per state?
![WOW2023_W31](https://github.com/chanronnie/Tableau/assets/121308347/6e4c416f-55d1-4c84-9548-0dbb78275675)

- View challenge: [#WOW2023 Week 31](https://workout-wednesday.com/2023w31tab/)
- View dataset: [Sample-Superstore 2022.2](https://github.com/chanronnie/Tableau/tree/main/WorkoutWednesday/%23WOW2023_W31/data)
- View my attempted recreation: [Tableau Link](https://public.tableau.com/app/profile/ronnie.chan/viz/WOW2023W31_16978377297050/WOW2023_W31?publish=yes)

# Covered Concepts
## Nested Level of Detail Expression (LOD) 

**Sales per State, Sub-cat**
```
{FIXED [State/Province], [Sub-Category]: SUM([Sales])}`
```

**Most Sold Sub-cat by State**
```
[Sales per State, Sub-cat] = {FIXED [State/Province]: MAX([Sales per State, Sub-cat])}
```

## Parameter (string)

**Select Sub-Category**

## Calculated Field 

**Selected Sub-cat**
```
IF [Sub-Category] = [Select Sub-Category ] AND [Most Sold Sub-cat by State]
THEN [State/Province] END
```

## Interactive Tooltip



https://github.com/chanronnie/Tableau/assets/121308347/5a6abeb8-613f-4c73-aa6c-4aa3ffb66d9c





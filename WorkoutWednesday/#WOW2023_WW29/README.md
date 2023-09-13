# #WOW2023 WEEK 29 - Blind Wine Tasting
<img src = 'https://github.com/chanronnie/Tableau/blob/main/WorkoutWednesday/%23WOW2023_WW29/image/wow2023_ww29.png'>

- View Challenge: [#WOW2023 Week29](https://workout-wednesday.com/2023w29tab/)
- View dataset: [here](data/Blind_Wine_Tasting_Results.csv)
- View my attempted recreation: [Tableau Link](https://public.tableau.com/app/profile/ronnie.chan/viz/WOW2023_WW29_BlindWineTasting/Dashboard1)

## Covered Concepts:
- Level of Detail Expression (LOD) </br>
`{FIXED [Taster]: SUM(IF [Wine Type] = 'White' THEN [Score] END)}`
- Image Role (URL) </br>
```
IF [Score Type] = 'Grape' 
THEN 'https://workout-wednesday.com/wp-content/uploads/2023/07/Grapes.png' 
ELSE 'https://workout-wednesday.com/wp-content/uploads/2023/07/Globe.png'
END
```
- Totals - SubTotals
- Sort records using a parameter
- Calculated Fields 
- Creating a "helper" column SIZE() to hold the total scores </br>
**Score Per Taster**: `{FIXED [Taster], [Wine Type]: SUM([Score])}` </br>
**Score on Total**: `IF SIZE() = 1 THEN SUM([Score Per Taster]) END`

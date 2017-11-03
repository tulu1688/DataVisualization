# Visualization fundamentals

## Defining Data Visualization
- First definition: Data visualization like mapping values to visuals
- Second definition: Data visualization is about turning numbers to pictures and stories. Allow us to explore and understand in a different way.

## Good data visualization
- Explanatory
- Exploratory

## Design code tell
- There're three skill need to have a good data visualization
  - Story teller
  - Design skill
  - Coding skill

## The Data Science Process
```
  Computer science       Static and Data Mining       Graphic Design       Infovis and HCI
|------------------|  |--------------------------|  |----------------|    |----------------|
acquire       parse   filtering            mining   represent   refine         interact
```

## Data types
- Quantitative data: continuous, discrete
- Categorical data
  - Nominal: ex: geographical region
  - Ordered:
    - ex: population bins (0-10 millions, 10-100 millions, 100-500 millions, >500 millions)
    - ex: class difficulty (easy, medium, hard)
- Question: Find the datatypes in ther image below
Inline-style:
![alt text](http://charliepark.org/images/slopegraphs/natgeo_scatter.jpg "Find the datatypes")
  - Answers:
    - Number of doctor visits per years: `order`
    - Life expectancy: `quantitative data`
    - Spending per person: `quantitative data`
    - Has health coverage: `nominal`

## Visual encoding
- Mapping `data` to `display elements`
- When visualize data has more than 2 dimension --> `retinal variables` is good method for visualizing other dimensions.
- An example of displaying types:
  - `Quantitative data` -> visualized by `position`
  - `Order data (retinal variables)` -> visualized by `size`
  - `geographical region` --> visualized by `color`
  - `time` --> visualized by `animation`
- Question: __World cup top scorer__ Find the visual encoding type for each variable![alt text](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57e9a59d_l1-worldcuptopscorers/l1-worldcuptopscorers.png "Find the visual encoding type for each variable")
  - Answer:
    - Country: position x
    - Goals scored: size
    - Player: position x
    - time: position y
    - top scorer: color hue
- Question: __Win, lose or draw__ Find the visual encoding type for each variable ![alt text](https://d17h27t6h515a5.cloudfront.net/topher/2016/September/57e9a683_l1-winloseordraw/l1-winloseordraw.png)
  - Answer:
    - Country: color hue
    - Game win/loses: position y / orientation
    - Scoring margin: position y / length
    - World cup winer: shape
    - Time: position x

## Ranking of visual encodings
- For quantitative variable
```
More accurate    Position
      ^            Length
      |            Angle / Slope
      |            Area
      v            Volume
Less accurate    Color / Den
```

## Up And Down The Visualization Spectrum
```
Productivity          WebGL, Canvas, SVG             Like assembly
      |                 |                       
      |                 v
      |               D3 js                          Like C/C++
      |                 |
      |                 v
      |             NVD3, Dimple js, Rickshaw        Like Python / Ruby
      |                 |
      |                 v
      v              Raw, Chartio, Tableau           Like Excel
```
- Notes: Rickshaw for time series

## D3 js
- D3: `Data Driven Documents`
```
Data         Driven        Documents
csv, json      ->          html
```
- D3.js web technologies: css, javascript, svg, html

# Chema Gálvez

## Description

People in Mexico has been suffering this violence for a long time but due to this, it's
sometimes difficult (or we normalize) to distinguished the size of the poblem.

I want to show (and makea an impact) on the historic violence Mexico has suffered over time with actual numbers.

## Technical Plan re: Option A/B/C/D

I'm planning to do Option A: Large Interactive using D3.js.

I want to make an interactive graph similar to the first two examples below, where the user inputs their birthdate
and then the graph will show how much homicides have happened since that date. In my case it would make sense
to have a bar chart rather than a line

### Inspiration:
- [How Much Hotter Is Your Hometown Than When You Were Born?](https://www.nytimes.com/interactive/2018/08/30/climate/how-much-hotter-is-your-hometown.html)
- [How much carbon was in the atmosphere when you were born?](https://www.nature.org/en-us/get-involved/how-to-help/carbon-footprint-calculator/carbon-by-birth-year/)
- [Reporte criminal de septiembre 2025](https://elcri.men/)

## Mockup

My idea is to make something close to my first source of inspiration. Each arrow in the sketch represents a transition:

[sketch](../sketch.pdf)

## Data Sources

### Data Source 1: Mortalidad INEGI (Mexico's Statistics Bureau)

URL: https://www.inegi.org.mx/sistemas/olap/proyectos/bd/continuas/mortalidad/defuncioneshom.asp?s=est

The data can be customized to add columns related to the characteristics of the homicide. For right now I have two different version of the data, divided by Sex and other divided by Age

- By age is a 32 x 7 df 
- By Sex is a 32 x 3 df

The data starts at 1990 and ends in 2022, 32 years of himicde statistics

### Data Source 2: Intentional homicides (per 100,000 people) - Mexico (World Bank)

URL: https://data.worldbank.org/indicator/VC.IHR.PSRC.P5?locations=MX

Same data as before but already normalized to homicides per 100,000 people.
Tbh I don't really like this presentation because it tends to minimize the problem rather than the raw numbers (at least for the average reader)

## Questions

1. When the user inputs their day of birth I will display the numer of homocides that happened in that year and after that I will show the cumulative homicides until 2022. I feel this is the correct way to not be misleading but I want your opinion on mixing the two different measurements. 
2. I know it's a small dataset but I feel like it's really relevant so I want to know if my idea gets a pass or if I a biger dataframe.
3. I really want to consider colors, I don't want this to turn into a political debate about presidents/parties because violence in Mexico for a long time has been sistematic rather that someone in particular fault. So other things that you may suggest to really pay attention to not make it biased or that it feels like it's directly attacking one or another government?
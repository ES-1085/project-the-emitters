Visualizing global and regional CO2 emmisions data over the course of recent history.
================
The Emitters

## Summary

After convening on our shared interests, we decided that climate data was something that we all found interesting as well as important to understand. We chose to specifically focus on emission data because it is one of the most important climate affecting values, while also being very quantitatively complex, thus allowing for more possibilities in research and visualization. We settled on the GHG emission dataset created by Our World in Data because of the sheer amount of data it contained, allowing us to visualize national emission data across the world for hundreds of years, as well as for the fact that it was already quite tidy and trustworthy. After some research it became clear that Our World in Data was simply an organization committed to making tidy data regarding important topics more accessible. The dataset itself is a collection of data from multiple different sources, the main ones being the Global Carbon Project, the Statistical Review of World Energy (BP), and International Energy Data (EIA).

When approaching this dataset, our question of research was this: How have national co2 emission trends evolved over time since the industrial revolution and what countries are the most responsible for creating the climate crisis? We set to answer this question by focusing on a specific few of the variables available in this dataset, primarily Country, Year, Population, GDP, and Co2. Our plan going into the project was to use these variables to create an animated spatial data visualization of the world, colored nationally by emission level. Along with that, we planned to use other visualizations such as histograms and scatter plots to visualize our research question in other ways.

We were curious to see what countries' growth rates in emissions looked like and how wealth impacts the growth or decrease of the rate. To visualize the trend, we used gganimate to create a dynamic geom_point from the end of WW2 to the present showing the annual difference in production-based CO2 emission for each country compared to the previous year. Countries are grouped into continents by colors, and the size of each dot represents the country's population size.  We discovered that the three wealthiest countries, China, United States, and India, also have the highest yearly increase in emissions, considerably higher than the rest of the world. 

Our data also had information on the total global emissions for other greenhouse gases (Nitrous Oxide, Methane, and CO2) and CO2 sources (oil, gas, and coal) for every year from 1990 until 2019. We used pivot_longer to get all the emissions into one column and their respective value into the other. We used an animated geom_bar to show the global yearly emissions for each GHGs or CO2 source, and we learned that all the analytes have increased at different rates, but coal, in particular, has almost doubled in the last three decades, with their emission exponentially increasing since 2000, which can be attributed to the economic development in China. The Asian country, since 2000, has massively increased its use of coal as a fuel for its highly demanded electricity.  We also learned that even though countries are trying to reduce global emissions, they are just steadily increasing.

Another core aspect of our project was creating maps of the world that reflect different countries contribution and responsibility towards climate change. We created labeled leaflet plots colouring countries by CO2 emission levels, as well as CO2 emissions per capita. We also wanted to incorporated GDP into our world map plots as a proxy for a countries ability to lower their emissions. We did this by creating a responsibility value that was a reflection of a countries carbon emissions per capita times their GDP per capita, and visualized this value on a world map animated over time. Through this animation we were able to see that countries such as Canada, the USA, Saudia Arabia, Australia, and Norway, have very high responsibility values with the USA having a consistently high responsibility value from the 1950s onwards.

Overall, through animated maps bar charts and scatter plots we were able to visualize the ways in which national co2 emission trends have evolved over time since the industrial revolution. In situations where outliers such as the United States and China made the scale difficult to differentiate the majority of countries, we used a scatter plot with logarithmically scaled axes to show the relation between all countries. We also had some success quantifying countries' responsibility towards the climate crisis, however none of the methods we utilized (ie. CO2 emissions, CO2 emissions per capita, and the reponsibility value that takes into account GDP) are perfect proxies for a countries' responsibility towards climate change. In reality, the situation is much more nuanced and difficult to justly quantify. GDP may be one way of determining a country's ability to mitigate their carbon emissions, but likely not the best or most fair way of doing so.


## Presentation

Our presentation can be found [here]([presentation/presentation.html](https://docs.google.com/presentation/d/18FdJH8AjCOKxJAkysUckcyhil2VZXAKmF_lORXVWm58/edit?usp=sharing)).

## Data

Ritchie, H, Roser, M, Mathieu, E, MacDonald, B, Rosado, P 2022, Data on CO2 and Greenhouse Gas Emissions, electronic dataset, Our World In Data, viewed January 12, 2023, <https://ourworldindata.org/co2-and-greenhouse-gas-emissions>

## References

Data on CO2 and Greenhouse Gas Emissions - Our World In Data
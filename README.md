<<<<<<< HEAD
Visualizing global CO2 emmisions data over the course of recent history
================
The Emitters

## Summary

Write-up of your project and findings go here. Think of this as the text
of your presentation. The length should be roughly 5 minutes when read
out loud. Although pacing varies, a 5-minute speech is roughly 750
words. To use the word count addin, select the text you want to count
the words of (probably this is the Summary section of this document, go
to Addins, and select the `Word count` addin). This addin counts words
using two different algorithms, but the results should be similar and as
long as you’re in the ballpark of 750 words, you’re good! The addin will
ignore code chunks and only count the words in prose.

You can also load your data here and present any analysis results /
plots, but I strongly urge you to keep that to a minimum (maybe only the
most important graphic, if you have one you can choose). And make sure
to hide your code with `echo = FALSE` unless the point you are trying to
make is about the code itself. Your results with proper output and
graphics go in your presentation, this space is for a brief summary of
your project.

## Presentation

Our presentation can be found [here](https://docs.google.com/presentation/d/18FdJH8AjCOKxJAkysUckcyhil2VZXAKmF_lORXVWm58/edit?usp=sharing). You can update this link to a Google Slides link.

## Data

Ritchie, H, Roser, M, Mathieu, E, MacDonald, B, Rosado, P 2022, Data on CO2 and Greenhouse Gas Emissions, electronic dataset, Our World In Data, viewed January 12, 2023, <https://ourworldindata.org/co2-and-greenhouse-gas-emissions>

## References

Our World in Data - Data on CO2 and Greenhouse Gas Emissions
=======
Visualizing global and regional CO2 emmisions data over the course of recent history.
================
The Emitters

## Summary

[Write-up of your project and findings go here. Think of this as the text
of your presentation. The length should be roughly 5 minutes when read
out loud. Although pacing varies, a 5-minute speech is roughly 750
words. To use the word count addin, select the text you want to count
the words of (probably this is the Summary section of this document, go
to Addins, and select the `Word count` addin). This addin counts words
using two different algorithms, but the results should be similar and as
long as you’re in the ballpark of 750 words, you’re good! The addin will
ignore code chunks and only count the words in prose.

You can also load your data here and present any analysis results /
plots, but I strongly urge you to keep that to a minimum (maybe only the
most important graphic, if you have one you can choose). And make sure
to hide your code with `echo = FALSE` unless the point you are trying to
make is about the code itself. Your results with proper output and
graphics go in your presentation, this space is for a brief summary of
your project.]

We were curious to see what countries' growth rates in emissions looked like and how wealth impacts the growth or decrease of the rate. To visualize the trend, we used gganimate to create a dynamic geom_point from the end of WW2 to the present showing the annual difference in production-based CO2 emission for each country compared to the previous year. Countries are grouped into continents by colors, and the size of each dot represents the country's population size.  We discovered that the three wealthiest countries, China, United States, and India, also have the highest yearly increase in emissions, considerably higher than the rest of the world. 

Our data also had information on the total global emissions for other greenhouse gases (Nitrous Oxide, Methane, and CO2) and CO2 sources (oil, gas, and coal) for every year from 1990 until 2019. We used pivot_longer to get all the emissions into one column and their respective value into the other. We used an animated geom_bar to show the global yearly emissions for each GHGs or CO2 source, and we learned that all the analytes have increased at different rates, but coal, in particular, has almost doubled in the last three decades, with their emission exponentially increasing since 2000, which can be attributed to the economic development in China. The Asian country, since 2000, has massively increased its use of coal as a fuel for its highly demanded electricity.  We also learned that even though countries are trying to reduce global emissions, they are just steadily increasing.

Another core aspect of our project was creating maps of the world that reflect different countries contribution and responcibility towards climate change. We created labeled leaflet plots colouring countries by CO2 emission levels, as well as CO2 emissions per capita. We also wanted to incorporated GDP into our world map plots as a proxie for a countries ability to lower their emissions. We did this by creating a responsibily value that was a reflection of a countries carbon emissions per capita times their GDP per capita, and visualized this value on a world map animated over time. Through this animation we were able to see that countries such as Canada, the USA, Saudia Arabia, Australia, and Norway, have very high responcibility values with the USA having a consistently high responcibility value from the 1950s onwards.

Overall, through animated maps bar charts and scatter plots we were able to visualize the ways in which national co2 emission trends have evolved over time since the industrial revolution. We also had some success quatifying countries' responsibilty towards the climate crissis, however none of the methods we utilized (ie. CO2 emissions, CO2 emissions per capita, and the reponcibility value that takes into account GDP) are perfect proxies for a countries' responsibility towards climate change. In reality, the situation is much more nuanced and difficult to justly quantify. GDP may be one way of determining a country's ability to mitigate their carbon emissions, but likely not the best or most fair way of doing so.





## Presentation

Our presentation can be found [here]([presentation/presentation.html](https://docs.google.com/presentation/d/18FdJH8AjCOKxJAkysUckcyhil2VZXAKmF_lORXVWm58/edit?usp=sharing)).

## Data

Include a citation for your data here. See
<http://libraryguides.vu.edu.au/c.php?g=386501&p=4347840> for guidance
on proper citation for datasets. If you got your data off the web, make
sure to note the retrieval date.

## References

List any references here. You should, at a minimum, list your data
source.
>>>>>>> 403e4a34f6134403a0449c6abb14607a01209310

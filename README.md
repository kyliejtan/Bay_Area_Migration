As you’ve sat in traffic on 280, stood on a crowded BART platform, or waited patiently in line at that new, highly rated brunch spot, have you ever wondered to yourself, “where the heck did all these people come from?” Most of us certainly have at one point in time or another, especially as we have seen, and felt the Bay Area get more and more crowded each year.

Since 2010, the population of the Bay Area has grown by over 600,000 people, an increase in population of roughly 8.5 percent, which is two and a half percent higher than the growth rate experienced by California as a state since 2010. This begs another question, why is the population of the Bay Area increasing at a higher rate than that of the rest of the state? When we consider this question, a number of reasonable hypotheses come to mind. From folks moving here to work in the Bay Area’s thriving tech sector, to its proximity to world-class nature and the vibrant, diverse communities that it’s home to, the Bay Area has had a powerful draw for many decades, and one that is likely due to an amalgamation of these wonderful features.

Gaining a more nuanced, more complete understanding of migration patterns to the Bay Area, and the potential reasons behind them is what this project was all about, and without further ado, here is what I found.

After cleaning, grouping, and sorting the data I collected by querying the US Census Bureau’s ACS Migration Flows API, I noticed a pretty interesting trend. San Francisco, Santa Clara, Alameda, San Mateo, and Marin counties all had the greatest number of people move into them from the same origin county, Middlesex County, MA. Additionally, a number of other counties reappeared amongst the top contributors to the populations of these five counties.

But what about the other five Bay Area counties?

While Contra Costa, Sonoma, Solano, and Napa counties do not exhibit the exact same trend in migration as the five aforementioned Bay Area counties, some similarities do still exist. Middlesex County, MA still appears amongst the top five contributors to two of the remaining Bay Area counties, and some of the counties that reappeared amongst the top contributors to the populations of the first five Bay Area counties also reappear amongst the top contributors to the remaining four.

These observed trends in migration to the Bay Area beg the following questions:
•	What similarities exist amongst Middlesex County, MA and the other counties that reappeared as top contributors to the populations of these five Bay Area counties?
•	What similarities exist amongst San Francisco, Santa Clara, Alameda, San Mateo, and Marin counties that could cause Middlesex County, Ma to be the top contributor to their populations?
•	What dissimilarities exist between the two groups of Bay Area counties that could cause them to experience different trends in migration?
•	Is this trend in migration observable in other US counties?

The answers: universities, tech, and it depends …

The common thread amongst all of the top contributors to the populations of the majority of Bay Area counties is that they are each home to at least one university or college, many of which happen to boast strong science, tech, and business programs. Middlesex County, MA
itself is home to Harvard, MIT, and Tufts University.

This realization really launched the rest of this project because it explains so much about why the observed migration trend into much of the Bay Area is the way it is. What we are seeing are the pipelines from the universities and colleges that feed the Bay Area’s tech and business sectors with new employees.

I feel like this also explaines the difference in migration patterns observed between the two groups of Bay Area counties. It makes sense that the more rural counties would see less of the pipeline effect because they are farther away from the nexus of Bay Area tech, as well as the diverse cultural centers and plethora of amenities that draw many to work in the Bay Area in the first place.

Time to put these theories to the test!

In order to better substantiate my theory that migration within the US is driven in large part by the pipeline between universities and areas with thriving tech and business sectors, I would need to expand the project’s scope to include counties outside of the Bay Area. I would also need to prove a correlation between some measurable aspect of the universities and colleges in each origin county and the number of people those origin counties contribute to migration into each destination county.

At this point we could look at more bar charts, but I appreciate the time you have taken out of your busy day to look at my work and I don’t want to waste it, so I’d like to instead jump ahead to something that I think is far and away more interesting.

Strength of origin county schools, explained.

I initially tried to correlate the highest world rank amongst all of the universities and colleges within each origin county with the number of people that county contributed to a given destination county. I came away with moderate correlations in a few cases, but the majority of correlations were rather weak. I think the problem with this approach was that a large portion of each origin county’s real-world contribution to each destination county’s workforce was being lost because only the strength of the top university in each origin county to produce desirable employees was being considered.

I think a more accurate description of the way this system works in reality is that all of the universities and colleges in an origin county contribute to that county’s ability to contribute new employees to migration into to a given destination county. Additionally, I think it’s reasonable to use a university or college’s rank as a measure for how much strength it contributes to an origin county’s total potential to contribute to migration.

To calculate the combined strength of an origin county’s schools to contribute to migration, I took the lowest world rank (Drexel University, #190) amongst the twenty four ranked universities and colleges of the combined eight origin counties, added 1, and then subtracted the rank of each university or college on the list from this number. This gave Drexel a strength score of 1, and Harvard a strength score of 187. The independent variables used in the graphs above are the sums of the strength scores of all of the ranked universities and colleges in each origin county

In summation.

Since the times of our earliest ancestors, people have migrated to new places for a variety of reasons, and even in today’s world, migration is still driven by many of the same reasons faced by our ancestors. The goal of this project was to gain a better, more nuanced understanding of the factors that drive migration into the Bay Area, and if I may be so bold, I feel like this project has been successful in achieving that goal.  I have shown through analysis of migration patterns captured by the US Census Bureau that pipelines from universities and colleges that supply new employees to the workforces of counties across the country account for a large part of the migration into those counties. I have also shown a strong correlation between the combined ability of the universities and colleges in an origin county and the number of people that county contributes to migration elsewhere.

My future goals for this project are:
•	To enhance its findings by measuring the degree of similarity between the migration patterns experienced by the counties I investigated in this project. My current plan to achieve this goal is to use One-Way ANOVA tests to measure the variance between the means of the migration patterns seen by each destination county.
•	I would then like to try to group these findings using a number of factors including the population size at the time of the Census Bureau’s survey, land area, and median household income of each destination county in order to tease out other factors that may influence the migration patterns into these areas.
•	Use Tableau, Plotly, and Leaflet to create more information-rich charts and maps of my results.

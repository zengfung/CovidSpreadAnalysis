Overall impression
==================

Summary of Report
-----------------

With COVID-19 cases still on a rise a year after it became a pandemic,
and with millions of cases and deaths throughout the world so far, we
wanted to find out whether the policies that were implemented during
this period of time were effective in slowing down the spread of the
disease. What caught our attention was the significant spike in cases
and deaths between October and November 2020 in European countries.
Hence, we analyzed the change in growth rate of infectious population
with respect to the stay-at-home restriction policy among five dense and
large European countries (Germany, France, Italy, United Kingdom, and
Poland). A panel fixed effect model was fitted, and it was found that
the stay-at-home policies did have a significant effect in reducing the
spread of COVID-19. However, model diagnostics have shown the issue of
cross-sectional dependence, which could lead to false positive error
inflation.

Overall Impression
------------------

The report was well-written in general. This was especially true for the
introduction and the background sections, as we managed to give a good
and engaging overview of COVID-19 to the readers and why the
stay-at-home policy is a good question of interest. Additionally, panel
regression also turned out to be a really good model for the purpose of
this analysis, as it explained the data at hand really well. The few
major constructive feedbacks that were received were the lack of legends
in certain bar charts making plots a bit harder to interpret, and that
the causal interpretation section felt disconnected from the previous
sections of the report. These issues will be further discussed in the
Major Comments section.

Major comments
==============

1.  The introduction section gave a good overview of the project,
    including a succinct and engaging description of the complex Covid
    19 situation, from brief background of the disease, its impact, and
    different non-pharmaceutical approaches that have been taken to
    control the spread of the disease. This transfers smoothly into the
    major question of interest of the study and the objectives. The
    readers could follow the report well and understand the thought
    process of the authors. It can be improved by breaking down the long
    paragraphs into shorter sections.

2.  The background section provided interesting insights on the problem
    of interest. The reason for choosing infectious population growth
    rate as the response variable was well explained and justified. The
    steps for deriving the response variable was also included and was
    helpful for readers who were not familiar with the disease spread
    SIR model.

3.  There was a big and long table in section 5.1.3. The table included
    the estimated regression coefficients and p-values for 28 variables,
    thus taking up a lot of space. Also it basically provided the same
    information as the line plot in the same section, so there was no
    need to include the table in the report.

4.  Several issues should be fixed to improve visualization:

    -   In Figures 1-4, the meaning of color is not shown in the report.
        We deleted the legend due to redundant legend when using Plotly.
        However, in the slide, we included a simple version of the
        legend.

    -   In the pie chart, Figure 5, the location of the five countries
        are not corresponding to geography. Thus, we adjusted the plot
        to be more consistent with what we see on a map.

    -   The y axis in Figures 1-4 using different ranges. Though we
        admit this can be confusing when using different units for five
        countries, we did not change the units since what we want the
        reader to see is the pattern (daily change over two months) for
        each country independently, rather than comparing each country’s
        absolute value.

5.  One of the major issues with the analysis was the causal
    interpretation. While a propensity score was run using the
    appropriate generalized Boosted model due to the variable being
    chosen not being binomial, the assumptions to run the propensity
    score were not stated. The model that was run seemed took into
    account many of the confounding variables. This was done by
    selecting data from a certain time interval and selecting certain
    countries. However, there were some assumptions that were made to do
    a propensity score analysis. One was that the countries had similar
    policies against COVID-19 in the selected time interval. These can
    include mask mandates, curfews, online schooling, and more.
    Differences in policies would lead to differing results in the
    analysis. For the presentation we will mention these assumptions and
    determine if causal interpretation can actually be made.

Minor comments
==============

1.  The tables we put on our report had too many decimal places. Some
    examples of this were the tables in Section 5.2, where we made a
    table that discusses the estimates of the model coefficients.
    Readers generally do not care to read beyond the 3rd decimal places
    as they don’t impact the results much anyway. In future reports,
    decimal places in tables should be reduced to at most 3 places.

Question to address during the final presentation
=================================================

1.  How do we interpret the fitted model that says that all stay-at-home
    policies, change in stay-at-home policies, and previous infectious
    population growth rate are significant?

2.  What does the Type-1 error inflation due to cross-sectional
    dependence mean for our results?

3.  What were the different cofounders that the model took into account?
    What variables weren’t taken into account?

4.  Why was a Generalized Boosted Model used to estimate the Propensity
    Score? What is the Generalized Boosted Model?

5.  What is the difference between change in stay at home restriction
    and stay at home restriction? Why was it important to have both?

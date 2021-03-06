# Belly Button Biodiversity

An interactive dashboard to explore the [Belly Button Biodiversity dataset](http://robdunnlab.com/projects/belly-button-biodiversity/), which catalogs the microbes that colonize human navels.

https://alapsraval.github.io/plotly-interactive-dashboard/

The dataset reveals that a small handful of microbial species (also called operational taxonomic units, or OTUs, in the study) were present in more than 70% of people, while the rest were relatively rare.

D3 library is used to read in `samples.json`.

## Step 1: A horizontal bar using Plotly

* A horizontal bar chart with a dropdown menu is created to display the top 10 OTUs found in that individual.

  * `sample_values` used as the values for the bar chart.

  * `otu_ids` used as the labels for the bar chart.

  * `otu_labels` uesd as the hovertext for the chart.

## Step 2: A bubble chart using Plotly

* A bubble chart is created to display each sample.

  * `otu_ids` used for the x values.

  * `sample_values` used for the y values.

  * `sample_values` used for the marker size.

  * `otu_ids` used for the marker colors.

  * `otu_labels` used for the text values.

## Step 3: Gauge Chart using Plotly

* The [Gauge Chart] (https://plot.ly/javascript/gauge-charts/) is used to plot the weekly washing frequency of the individual.

## Step 4: Metadata and drop down filter using D3

* The sample metadata is displayed under Demographic Info.

* The chart is updated whenever a new sample is selected.

### About the Data

Hulcr, J. et al.(2012) _A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable_. Retrieved from: [http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/](http://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)

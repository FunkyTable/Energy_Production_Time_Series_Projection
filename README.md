# Achieving Paris Agreement Goals: Projecting Energy Production Sources in the United States With Time Series Modeling
 
## Overview
The United States needs to achieve Paris Agreement greenhouse gas reduction goals in the energy production sector by 2050. The nation must understand current trends in the sector to see if EPA intervention is required to meet the targets. This project projects current energy production trends in the United States and recommends changes to achieve the Paris Agreement reduction goals.

## Business Problem

### Background: 
On December 12, 2015, the historic [Paris Agreement](https://apnews.com/article/climate-climate-change-john-kerry-paris-archive-81dabae32cb8463b86bd85d762da9e6d) legally bound the United States and other nations of the world to limit global warming to well below 2 °C (3.6 °F) over preindustrial levels. 

The Paris Agreement also commissioned the Intergovernmental Panl no Climate Change ([IPCC](https://www.ipcc.ch/)) to review the effects of climate change at 1.5 °C (2.7 °F). [The IPCC released its report on the matter in 2018](https://www.ipcc.ch/sr15/chapter/spm/), detailing the pestilence of a warmer world. 

To limit climate change to no greater than 1.5 °C over pre-industrial levels, the IPCC's 2018 special report concluded that greenhouse gas (GHG) emissions must ["decline by about 45% from 2010 levels by 2030 (40–60% interquartile range), reaching net zero around 2050."](https://www.ipcc.ch/sr15/chapter/spm/#article-spm-c) Today, in 2023, we are [already at 1.1 °C (2 °F)](https://earthobservatory.nasa.gov/world-of-change/global-temperatures). With GHG emissions as they are, scientists anticipate this average to grow by about 0.2 °C per decade unless GHG emissions are cut.

### Buisness Problem: 

The United States needs to ensure our energy production sector achieves the Paris Agreement goals. 

GHG emissions occur in multiple sectors of the economy. Electricity generation releases [about 25% of GHG emissions in the United States](https://www.epa.gov/ghgemissions/sources-greenhouse-gas-emissions), [and about 40% globally](https://www.iea.org/data-and-statistics/charts/global-energy-related-co2-emissions-by-sector). The EPA commissioned Greg Osborne to project current energy production trends and recommend policies to help the United States reach the GHG reduction targets set by the IPCC. 

Electricity generation refers to power plants creating electricity to distribute across power lines to residential and business locations. Electricity sources include fossil fuel methods, burning coal, oil and natural gas which emit GHG, and sources that do not emit GHG, nuclear, wind turbines, solar panels and hydroelectrical. Reducing America's GHG emissions and exporting that technology to our allies will result in greater reduction of GHG emissions than any other sector.

## Time-Series Modeling

The time series analysis requires projecting two factors into the future:

   **1. Construction/Reduction Rate of GHG-Emitting Power Generation**

Unfortunately, not only are fossil fuels still powering our lifestyles, but power companies in the US still [plan to open natural gas power plants in future](https://www.eia.gov/todayinenergy/detail.php?id=50436). Construction of new coal plants has [stalled in the United States](https://www.scientificamerican.com/article/will-the-u-s-ever-build-another-big-coal-plant/), but worldwide, several coal-fired power plants are scheduled to be [built in the future](https://www.reuters.com/business/energy/cop26-aims-banish-coal-asia-is-building-hundreds-power-plants-burn-it-2021-10-29/). The time series analysis must consider the growth and reduction of fossil-fuel power plants.

   **2. Construction Rate of Clean Power Generation**

Contrary to what the crisis needs, we cannot build a billion wind turbines overnight. We can only build clean energy sources as materials, labor availability, construction time, and politics allow. Fortunately, construction of new renewable and nuclear power production is underway. The time series analysis will model current trends of construction to see if they can meet the The United State's electricity needs as fossil fuels diminish.

I will then compare this time series analysis with two other factors that are not projected with a time series model:

   **1. Increase in Electricity Demand**

America's demand for electricity will rise as we cut emissions across all sectors. The poster-child example of this is the impending fuel source change for automobiles. Car manufacturers representing a quarter of global sales have pledged to [cease production of internal-combustion-engine cars](https://www.caranddriver.com/news/a38213848/automakers-pledge-end-gas-sales-2040/) within the IPCC's timeline. The most likely power source for their new cars is electricity, creating greater demand. The data used to estimate the increase in Electricity demand is provided by the International Energy Agency.

   **2. The Paris Agreement GHG Emissions reduction targets**

As part of the Paris Agreement, the IPCC has determined that GHG emissions must ["decline by about 45% from 2010 levels by 2030 (40–60% interquartile range), reaching net zero around 2050"](https://www.ipcc.ch/sr15/chapter/spm/#article-spm-c). To simulate this in the electricity production industry, I have defined this reduction as an overall reduction in electricity power generation for each fossil fuel energy production source (coal, oil and natural gas). These reduction targets are visible in the graphs produced in this report.

With all these factors, time-series modeling can assist with projection needs. This project will show the United State's energy production trends, and make recommendations for how to achieve the Paris Agreement Goals.

Compared with the random walk baseline model, the selected models achieved its goal of realistically projecting construction / reduction trends in the electricity generation sector.

## Methodology

The planned steps I will follow for this project include: 

   1. Create a time series models that project energy production trends for each fuel source in the United States to the year 2050. 
   2. Plot all energy production trends against the projected energy demands of the United States.
   3. Using interpolation, determine what reductions and construction increases are necessary to achieve the Paris Agreement goals. This will not use time series, as it's a determination of what trends must accomplish, rather than where the trends will go if left unchecked.

## Data Understanding and Analysis
1. Sources of data
      * Energy Production Wattage by Country by Source: [Our World In Data](https://ourworldindata.org/grapher/electricity-prod-source-stacked)
        * Original source: [BP](https://www.bp.com/en/global/corporate/energy-economics/statistical-review-of-world-energy.html)
      * Historic Electricity Demand by Country: [Our World In Data](https://ourworldindata.org/grapher/electricity-demand?country=USA~GBR~FRA~DEU~IND~BRA)
        * Original source: [BP](https://www.bp.com/en/global/corporate/energy-economics/statistical-review-of-world-energy.html)
      * Energy demand projection up until 2050: [IEA](https://www.iea.org/data-and-statistics/data-product/world-energy-outlook-2022-free-dataset)
        * Data sourced from the IEA's World Energy Outlook 2022 Report: [Countries by Region](https://iea.blob.core.windows.net/assets/830fe099-5530-48f2-a7c1-11f35d510983/WorldEnergyOutlook2022.pdf#page=499)

3. Visualizations
    WORK IN PROGRESS - EVERYTHING BELOW IS A PLACEHOLDER
  Eight visualizations that are also in the notebooks.
    * ![Confusion Matrix](Visualizations/ConMatrix.png)
    * ![True Targets vs. Predicted Targets](Visualizations/TrueVsPred.png)
    * ![Word Associations : Google](Visualizations/WA-Google.png)
    * ![Word Associations : Android](Visualizations/WA-Android.png)
    * ![Word Associations : Android](Visualizations/WA-Android-Negative.png)    
    * ![Word Associations : Apple](Visualizations/WA-Apple.png)
    * ![Word Associations : Google](Visualizations/WA-iPad.png)
    * ![Word Cloud](Visualizations/WordCloud.png)
  Five graphics exclusively for aesthetics in the Google Slides doc.
    * ![Crowd](Visualizations/Crowd.jpg)
    * ![Commission](Visualizations/Commission.jpg)
    * ![Data Science](Visualizations/DataScience.png)
    * ![NLP](Visualizations/NLP.png)
    * ![Questionmark](Visualizations/Questionmark.jpg)

## Conclusion
WORK IN PROGRESS


## Repository Structure
WORK IN PROGRESS - EVERYTHING BELOW IS A PLACEHOLDER

```
  ├── Visualizations : images used in PPT and readme
├──Notebook-Word-Associations.pdf : PDF copy of Notebook for testing Data
├──Notebook.pdf : Print of main Jupyter Notebook used for modeling 
├──Presentation.pdf : Presentation for Stakeholders
├──README.md : Project information and repository structure
├──github.pdf : PDF of repository
├──judge-1377884607_tweet_product_company.csv : The raw data analyzed
├──Student-Word2Vec-Workspace.ipynb : Jupyter Notebook for testing Data
└──Student.ipynb : Jupyter Notebook

```

# Readme should include (Copied from Assignment Objectives):


**Still missing from this README**
3. A **header image**
    * This image can be anything you want, so long as it is professional and aligns with your project
    * Ideal dimensions are 1280x640 pixels, but any image with landscape orientation (wider than it is tall) will work
    * Image sourcing ideas to consider:
      * Use a stock image from a source like [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) or [Unsplash](https://unsplash.com/)
         * Make sure you double-check the usage license and attribution requirements
      * Create visualizations with code (Matplotlib, Seaborn, etc.)
      * Take your own photo
         * This is most relevant if you have a real-world connection to the domain
    * As a reminder, the Markdown notation for an image is `![alt text](path/to/image.png)`
    
6. **Conclusion**
    * How would you recommend that your model be used?
7. **Repository Navigation**
    * An explanation of the repository organization
    * Links to the final notebook and presentation
       * As a reminder, the Markdown notation for a link is `[link text](/path/to/file)`
    * Reproduction instructions (or a link to them)


Ideally, your README should include:

1. A **project title**
    * Choose a title that reflects the project domain and presents you as a data scientist, not as a student. The title should not include words like "capstone" or "school"
    * Some title formats to consider:
       * "Predicting `target`"
       * "`target` Prediction"
       * "`target` Detection"
       * "Classifying `target`"
       * "`target` Recommender"
       * etc.
    * Feel free to add "with `data`" or "using `data`" to the end of any of those. For example, *Detecting Fake Reviews with NLP* or *Classifying Skin Lesions Using Neural Networks*
    * You also might want to start the title with a catchy phrase or quote, followed by a more-standard title. For example, *Where To, First?: an Airbnb Destination Predictor* or *Stay in Your Lane! Automated Bike Lane Enforcement*
      * You can always add this element later, so don't get hung up on it if you can't think of something right away! Just start with the straightforward title
2. An **elevator pitch**
    * Immediately after the title, write a very short description of the problem you are solving, the data you are using to solve it, and how well your model solves the problem
    * This should be no more than a couple of sentences
3. A **header image**
    * This image can be anything you want, so long as it is professional and aligns with your project
    * Ideal dimensions are 1280x640 pixels, but any image with landscape orientation (wider than it is tall) will work
    * Image sourcing ideas to consider:
      * Use a stock image from a source like [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page) or [Unsplash](https://unsplash.com/)
         * Make sure you double-check the usage license and attribution requirements
      * Create visualizations with code (Matplotlib, Seaborn, etc.)
      * Take your own photo
         * This is most relevant if you have a real-world connection to the domain
    * As a reminder, the Markdown notation for an image is `![alt text](path/to/image.png)`
4. **Business Understanding and Data Understanding**
    * Explain the project context, using at least one citation to demonstrate your domain understanding
    * Consider including visualizations here as well
5. **Modeling and Evaluation**
    * What kind of model(s) did you use?
    * How well did your final model perform, compared to the baseline?
6. **Conclusion**
    * How would you recommend that your model be used?
7. **Repository Navigation**
    * An explanation of the repository organization
    * Links to the final notebook and presentation
       * As a reminder, the Markdown notation for a link is `[link text](/path/to/file)`
    * Reproduction instructions (or a link to them)

The best practice would be to include all of the items listed above in your README. Items 2 and 7 are particularly relevant for grading, as described below.
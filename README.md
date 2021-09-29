# Daniel Huang 

Welcome to my Github! 

My name is Daniel Huang, and I am 21 years old. I am currently a first year M.A. student studying Statistics at UC Berkeley, and I graduated from UMass Amherst with a B.S. in Statistics and minor in Computer Science. I'm passionate about using data to solve problems and gain valuable insights. I have passed Actuarial Exams P and FM, and have worked with mostly P&C insurance data through my 2 internships with Travelers Insurance. I'm eager to expand my horizons and am excited to see what types of data I can work with next!

# Projects
## Honors Thesis
I wrote my honors thesis supervised by Professor Panagiota Birmpa and Professor Markos Katsoulakis on Uncertainty Quantification in Conditional Random Field Models for Optical Character Recognition. My thesis uses uncertainty quantification techniques, specifically utilizing the Donsker-Varadhan Representation of the KL-Divergence as a measurement of the distance between my base model built in Python with other models. 

## Home Pricing Model
I worked to create a multilinear regression model in R to predict home prices in Oregon utilizing both quantitative and qualitative predictors. After performing preliminary data exploration to find relationships between predictors, I implemented techniques such as Stepwise AIC and BIC regression, F-tests, and outlier analysis to create the final model. My model was able to predict 60% of the variation in home prices given the data.


# Coding Samples

## Lyric Finder
R function to pull lyric, album, and song artist from mldb.org based on a song and title. Utilizes string manipulation to build the get request URL for the desired page, then uses the rvest package to scrape the desired data.

## State of the Union Speech Webscraper
R function to pull information about the State of the Union speeches from the UCSB database. Utilizes lapply to vectorize data cleaning and extraction for each speech. We build a data frame of speeches with the President, date, as well as key metrics about the speech such as word count and average word length. The unspoken parts of the body of the speech are stripped and saved, and the body of the speech is prepared for analysis. Using Regex, we find words/wordstems of interest and calculate their frequencies. This allows us to see the progression of certain metrics of interest over time. We also allow grouping by political party. Packages used include stringr, dplyr, and rvest.

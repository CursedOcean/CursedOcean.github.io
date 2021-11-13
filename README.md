# Daniel Huang 

Welcome to my Github! 

My name is Daniel Huang, and I am 21 years old. I am currently a first year M.A. student studying Statistics at UC Berkeley, and I graduated from UMass Amherst with a B.S. in Statistics and minor in Computer Science. I'm passionate about using data to solve problems and gain valuable insights. I have passed Actuarial Exams P and FM, and have worked with mostly P&C insurance data through my 2 internships with Travelers Insurance. I'm eager to expand my horizons and am excited to see what types of data I can work with next! Please feel free to look around at my projects and coding samples to get an idea of what skills I have and what I'm passionate about. You can reach out to me at dhuang172@gmail.com if you're interested in working together!

## Technical Skills
I am fluent in R, Python, and SQL, with academic experience using Java, C++, and Unix-style environments. I'm familiar with most R packages, including dplyr, ggplot2, and the rest of the tidyverse. In Python, I have worked with Numpy, Pandas, and briefly with some machine learning packages from scikit-learn. I have corporate experience with ArcGIS, as well as the standard suite of Microsoft tools (Excel, Word, and Powerpoint). I'm eager to learn, and willing to work hard to pick up new skills.

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

## Remote Linux Cluster Parallelization using R
R and Bash code to utilize UC Berkeley's remote SCF Cluster to perform parallelized processing of Wikipedia data related to Barack Obama. Utilized the Futures package in R in order to read in and process Wikipedia data in parallel remotely. Results stored in Obama2.csv, and brief analysis done. Next coding sample has more in-depth analysis and results.

## Remote Linux Cluster Parallelization using Dask in Python
R, Bash, and Python code again using UC Berkeley's remote SCF Cluster to performed parallelized processing of Wikipedia data related to Barack Obama, specifically from Aug 2008 to Dec 2008, when he became president for the first time. Roughly 120 GB of zipped data are processed in parallel using Python's Dask package, and the number of hits on pages containing 'Barack_Obama' is aggregated for each Day-Hour from Aug 1 2008 to Dec 31 2008. The data are then exported as a csv to be analyzed in R with graphs using the ggplot2 package.


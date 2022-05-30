# Daniel Huang 

Welcome to my Github! 

My name is Daniel Huang, and I am 22 years old. I am currently working as a Technical Analyst at Wayfair. I got my M.A. in Statistics at UC Berkeley, and I graduated from UMass Amherst with a B.S. in Statistics and minor in Computer Science. I'm passionate about using data to solve problems and gain valuable insights using machine learning. I have passed Actuarial Exams P and FM, and have worked with mostly P&C insurance data through my 3 internships with Travelers Insurance. I'm eager to expand my horizons and am excited to see what types of data I can work with next! Please feel free to look around at my projects and coding samples to get an idea of what skills I have and what I'm passionate about. You can reach out to me at dhuang172@gmail.com if you're interested in working together!

## Technical Skills
I am fluent in R, Python, and SQL, with academic experience using Java, C++, and Unix-style environments. I'm familiar with most R packages, including dplyr, ggplot2, and the rest of the tidyverse. In Python, I have worked with Numpy, Pandas, and scikit-learn. I have coded from scratch as well as utilized out-of-the-box packages for machine learning algorithms such as Linear Regression, SVM's, Random Forest, and gradient boosted models. I have corporate experience with ArcGIS, as well as the standard suite of Microsoft tools (Excel, Word, and Powerpoint). I'm eager to learn, and willing to work hard to pick up new skills.

# Projects
## Master's Capstone
My capstone project is titled Credit Card Fraud Detection Using Machine Learning Methods. Using a Kaggle dataset (https://www.kaggle.com/competitions/ieee-fraud-detection/overview), my team and I built Logistic Regression and Random Forest models to detect fraudulent transactions. We utilized identity information about users that other Kagglers had not done before, and were able to show that our models that utilized this identity information performed better than models without. We were further able to quantify this improvement and provide a business recommendation as to how much companies would save by having identity information for a given transaction. Our code is in a Jupyter Notebook and the attached writeup is included as well.

## Housing, Health, and Happiness Replication Paper
I carried out a replication of the results found in the paper Housing, Health, and Happiness by Catteano et al. By rewriting the code using R and re-running all of their analysis using provided data, I was able to replicate their results as well as robustness checks. Furthermore, I conducted additional analysis using leave-one-out-errors as well as leverage score analysis. While the leave-one-out-errors were fairly robust, I found that there were a few specific data points that had extremely high leverage, and leaving them out dramatically altered some of the results, specifically the cluster robust standard errors. The writeup is attached with code at the end.

## Honors Thesis
I wrote my honors thesis supervised by Professor Panagiota Birmpa and Professor Markos Katsoulakis on Uncertainty Quantification in Conditional Random Field Models for Optical Character Recognition. My thesis uses uncertainty quantification techniques, specifically utilizing the Donsker-Varadhan Representation of the KL-Divergence as a measurement of the distance between my base model built in Python with other models. 

## Genetic Algorithm Variable Selection Package for Linear Models and GLMs in R

Installable R Package named GA that does genetic algorithm variable selection for LM and GLM models. Variable selection will be done using default using the AIC criterion, but users can define their own fitness functions for the algorithm to use. Other user-inputted features include crossover functions, mutation rate, and other selection algorithm options. Unit testing and full examples included to demonstrate utilization of the package, as well as documentation created using the roxygen2 package.

Genetic algorithm overview: Genetic algorithms are utilized to simulate the process of Charles Darwin's theory of natural selection. The fittest individuals, with respect to their genetic code, in a population are chosen to reproduce and their offspring make up the next generation. Reproduction among fit individuals results in desirable traits and attributes being passed down to future generations. Reproduction involving less fit individuals along with genetic mutations ensures that we have a diverse population. This process of pairing individuals for reproduction continues until the algorithm decides that the current generation has converged to the best level of fitness. Within our implementation of this genetic algorithm, there are five main steps that we consider: 1) generating our initial population, 2) evaluating the fitness of individuals, 3) selecting pairs of parents via a selection mechanism, 4) perform a crossover of the two parents chromosomes to produce two children for the next generation, and 5) allow for a small chance of mutation to increase genetic diversity. In this R package, we utilize a genetic algorithm for variable selection for linear regression and generalized linear models. Our package was designed in accordance to Hadley Wickham's guide for R packages.

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

## EM Algorithm for Censored Regression
R code implementing EM Algorithm for simple linear regression with right censored data i.e. for y values greater than some c, we only have the censored value c not the actual value. We utilize the expectation-maximization algorithm in order to average over these unknown data in our regression process. Results compared to direct optimization of the log-likelihood for normal regression coefficients.

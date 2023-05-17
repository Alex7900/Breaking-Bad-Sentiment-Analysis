# Breaking Bad Sentiment Analysis
Performing sentiment analysis of lines spoken by Walter about Jesse in the show Breaking Bad.

### Introduction
I will walk through the steps for analyzing the sentiment of lines spoken by Walter about Jesse in the show Breaking Bad. The goal is to understand the factors influencing the sentiment of these lines, calculate a linear regression model, and observe changes in sentiment across different seasons. (Season 3 only until Episode 7 included due to tidyness issues)

### Step 1: Load the transcripts and extract lines
We start by loading the transcript files for each season. In my example, I used the first three seasons (S03E07), but you can add more seasons by updating the transcript_files list.

### Step 2: Extract lines spoken by Walter about Jesse
For each seasons transcripts, I use a regular expression pattern to extract lines spoken by Walt. I then filter these lines to keep only those that mention "Jesse".

### Step 3: Sentiment analysis using VADER
I use the VADER sentiment analysis tool to compute sentiment scores for each line mentioning Jesse. VADER returns a compound sentiment score, which we store in a dataframe along with relevant information, such as line length, number of words, and the presence of the word "Jesse".

### Step 4: Fitting a basic linear model
I fit a basic linear regression model to the data to determine factors influencing sentiment. I use line length, number of words, as explanatory variables.

### Step 5: Calculating the average sentiment and Rate of Change (ROC) of sentiment for each season
I calculate the average sentiment and ROC of sentiment from the lines mentioning Jesse for each season and graph them out to see precisely the changes in sentiment from Walt

### Outcomes
By running this code, we can gain insights into the relationship between Walter and Jesse as the story progresses. We can explore how their relationship evolves, identify any significant shifts in sentiment related to key plot points or character developments, and understand the factors influencing sentiment in their interactions.

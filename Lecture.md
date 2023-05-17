## Applying DA in Marketing

Analysis Techniques

#### 1. Causal Analysis
- Finding cause and find correlation
<pre>
## Problem : 
- Hard to tell if it is causality or correlation
- Bias during the experiment

## Solutions :
- Randomized Experiment : Not always easy to conduct
- Observational Approaches (Quasi-experiment) : Before vs After
  : Exogenous shock 
  : Exclusion restriction
</pre>

#### 2. Survey Analysis
- Ex : Customer satisfaction
<pre>
## Attention point
- Psychological  constructs (Attitude, Emotions, Attitude Strength, etc.)
- Proper measurement (Surveys, Text/Image Analysis, Network Analysis)
- Varying targets (Products, Services, Companies/Brand)
- Differences in the impact of individuals's expressions
- Satisfaction changed over time

## Types of Data
- Survey data
- Social media data
- Online behavioral data
And more
</pre>

#### 3. Statistical Analysis
- T-tests : Comparing averages of 2 scores if they are similar
- Multiple linear (Continuous or trends) | Logistic regression (0 or 1)
- Machine learning

#### 4. Text Analysis
Example : Twitter Positive-Nagative Top 10 analysis (Analyzing Social Media Attitudes Part 2)
<pre>
1) Collect text data
2) Tokenize the text (Capturing words by word by computer) 
3) Normalize the tokens (Ex : remove underscore, delete !, etc.)
4) Remove stop words (or, and, the, this, etc.) but not neccesary
5) Stem tokens (Running, ran, runs -> run)

After cleaning we can
- Frequency Counting
- N-grams frequency counting (Unigram - Love, Bigram - Love you, Trigram - I Love you)
- Using packages in R
</pre>


LDA Topic Modeling
- Go through each document, and randomly assign each world in topics
  : Ex Topic 1 - dog, tree, green, Topic 2 - spider, guy, pizza
- Improve to group the words better (by repeating again and again) then name the topic by human
  : Ex Technology -> computer, data, bitcoin
  
<pre>
For example : Steps on Tweets LDA Analysis
1. Read CSV file (or other sources)
2. Cleaning (Remove URL, Tokenize, Normalize, Remove stop words)
3. Create a Document-term Matrix
4. Run LDA
5. Plot top terms by topics
</pre>

#### 5. Network Analysis
- Social media data
- Relationship between people
Using <strong>Network graph</strong> to represent relationships between nodes

<pre>
Terms 
- Clique : Interesting group of nodes, All nodes must be connected
- Cluster : Connected Groups of nodes (huge group)
            connecting between groups call "Bridge"
</pre>

Analyzing Influence
<pre>
Attention :
- Bridge
- Centrality
- Deegree Centrality (number of ties on a node) : in/out degree
- Closeness Centrality : average of the shortest paths from one to all other nodes
- Eigenvector Centrality***
</pre>

<pre>
Example : Twitter analysis for the influence of individuals
Possible Ties : Number of Retweets, Follow, Mentions
***See R code in the local machine*** 
</pre>









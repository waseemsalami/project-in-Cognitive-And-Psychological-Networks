# project-in-Cognitive-And-Psychological-Networks
Comparative data analysis of semantic networks between two personality types based on the 'MBTI' personality test, which are INFJ - ENFJ

# Informative background describing the phenomenon:
The MBTI personality test distinguishes and classifies personalities based on four dichotomous dimensions:

  1. Introversion (I) / Extroversion (E)
  2. Intuition (N) / Sensing (S)
  3. Thinking (T) / Feeling (F)
  4. Judging (J) / Perceiving (P)

The two personality types we chose to focus on are:
ENFJ – Extroverted Intuitive Feeling Judging
INFJ – Introverted Intuitive Feeling Judging
It can be seen that these two personality types differ only in the first dimension, Introversion (I) / Extroversion (E).

The reason we chose to compare these two types is that we are interested in examining the difference between semantic networks of introverted individuals compared to extroverted individuals. We are also interested in understanding the impact of introversion/extroversion on our personalities. We thought that if we take two individuals whose personalities are "similar" in every dimension except for the dimension of introversion/extroversion, we can more precisely separate and compare them, and also compare our results with the research findings based on this personality test.

# Data Collection:
We will collect textual data from the subreddits of the two personalities:
INFJ Personality: https://www.reddit.com/r/infj
ENFJ Personality: https://www.reddit.com/r/enfj
Data collection will be performed using the Reddit API.

Objective and Research Questions:
Investigating the semantic structure of these two different personality subreddits raises several interesting research questions:

## Primary Research Question: How do the semantic networks of individuals with introverted personalities differ from the networks of individuals with extroverted personalities?

Secondary Research Questions:
2. How do the semantic networks of individuals with INFJ personalities differ from the networks of individuals with ENFJ personalities?

Does personality type influence the organization of the semantic network?

In all questions, it is also possible to incorporate a check for correlation with the findings of the MBTI research.

# Nodes, Edges, and Structure of the Network:

The semantic network representing each personality type will be a Word Co-Occurrence Network, an undirected graph. In this network, nodes will be defined as common words within the subreddit, such as the 50 most frequent words representing the top 50 words used in that subreddit. Edges will be created between words that co-occur frequently in the same post or sentence, indicating a significant relationship. 

The weight of the edge between two words will be defined as the Occurrence-Co measure of these words. This measure represents the frequency of the common occurrence of two words, taking into account the size of the dataset and other relevant factors. Essentially, the weight will quantify the extent of the shared appearance of the two words.

For example, in the INFJ subreddit, words like "Introvert" and "Social" might be among the most frequent, and the edges between them will represent the common appearance in many posts discussing social situations that introverted individuals find themselves in. Similar patterns can be observed for other word pairs such as "Social" and "Anxiety."

In the ENFJ subreddit, a parallel exploration might reveal similar patterns but with different word pairs, for instance, "Extrovert" and "Social."

Analyzing the Word Co-Occurrence Network in this manner allows for a deeper understanding of the semantic structure within each personality type's subreddit and facilitates the comparison between them.

# Data Processing:
Natural Language Processing (NLP) and machine learning algorithms will be employed to preprocess the text data. After preliminary processing, semantic networks will be constructed for each group.

# Analysis:
The semantic networks will be analyzed using various metrics such as cluster coefficient, centrality measures, and average shortest path length. Identifying communities will help pinpoint groups of related concepts within the network. Additionally, efforts will be made to recognize patterns and structural differences between the networks representing the two groups.

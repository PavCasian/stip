# High-risk high-reward research exploratory analysis
This short piece of analysis focuses on **high-risk high-reward research**, which is defined as research that involves a substantial level of risk due to its high degree of novelty and uncertainty. However, if it's successful it will have a significant impact in solving complex problems. The main questions this analysis looks to answer are:

1. What is the distribution of high-risk high-reward research initiatives per year?
2. Which policy instrument types have been used in high-risk high-reward research initiatives and how frequently?
3. What's the budget allocation for each policy instrument type used in high-risk high-reward research initiatives? 

To address these research questions, this analysis leverages the OECD’s [STIP Compass dataset](https://stip.oecd.org/stip/). While the STIP Compass is a premier resource for science, technology, and innovation policy, its data requires careful interpretation due to inherent reporting variations. Notably, inconsistencies in the granularity of data provided by different countries may impact [cross-national comparability](https://stip.oecd.org/stip/pages/about).

It's worth mentioning some of the high level characteristics of the dataset:
a. Columns are roughly classified in four groups:
  - Policy initiatives - includes initiative ID, country, budget range and other information relevant at the initiative level
  - Themes - initiatives are classified in themes, such as high-risk high-reward research; theme columns have the "TH" prefix
  - Target groups - initiatives have at least one target group, such as academic societies / academies; these have the "TG" prefix
  - Policy instruments - initiatives are enacted through instruments, such as project grants for public research; most of these have the "F" prefix
b. One row in the dataset represents a policy instrument type. Note that a policy initiative can have from one to several instrument types
c. The second row in the dataset is a description column for the first row of the dataset, which means that the actual data starts from the third row down

More information about the dataset can be found on the [STIP Compass](https://stip.oecd.org/stip/) website.

<h1 align="center">High-risk high-reward research exploratory analysis</h1>

This short piece of analysis focuses on high-risk high-reward research, which [OECD](https://stip.oecd.org/stip/interactive-dashboards/themes/TH23) defines as research involving a substantial level of risk due to its high degree of novelty and uncertainty but with significant potential in solving large and complex problems.  

The main questions this analysis looks to answer are:
1. What is the distribution of high-risk high-reward research initiatives per year?
2. Which policy instrument types have been used in high-risk high-reward research initiatives and how frequently?
3. What is the budget allocation for each policy instrument type used in high-risk high-reward research initiatives? 

To address these questions, the analysis leverages OECD’s [STIP Compass dataset](https://stip.oecd.org/stip/). While STIP Compass is a premier resource for science, technology, and innovation policy, its data requires careful interpretation due to inherent variations occuring during data collection. Notably, inconsistencies in the granularity of data provided by different countries may impact [cross-national comparability](https://stip.oecd.org/stip/pages/about).

It's worth mentioning some of the high level characteristics of the dataset:
- Columns are roughly classified into four groups:
  - Policy initiatives - includes initiative ID, country, budget range and other information relevant at the initiative level
  - Themes - initiatives are classified in themes, such as high-risk high-reward research; theme columns have the "TH" prefix
  - Target groups - initiatives have at least one target group, such as academic societies / academies; these have the "TG" prefix
  - Policy instruments - initiatives are enacted through instruments, such as project grants for public research; most of these have the "F" prefix
- One row in the dataset represents one policy instrument type used in an initiative. Note that a policy initiative can have from one to several instrument types
- The second row in the dataset is a description column for the first row of the dataset, which means that the actual data entries start from the third row down

More information about the dataset can be found on the [STIP Compass](https://stip.oecd.org/stip/) website.

<h2 align="center">Outcome</h2>
<h3>Question 1: What is the distribution of high-risk high-reward research initiatives per year?</h3>

<img width="1189" height="453" alt="time_series" src="https://github.com/user-attachments/assets/28ff6a07-416d-4733-9bb1-175caf54e406" />

There has been a visible increase in high-risk high-reward initiatives over the last decade. However, since STIP Compass was [launched in 2018](https://one.oecd.org/document/DSTI/STP(2018)8/en/pdf), it is possible that older initiatives were not fully captured retrospectively. To confirm whether this trend reflects a real policy shift or is simply a result of more recent data collection, it would be beneficial to cross-reference these findings with other data sources.

<h3>Question 2: Which policy instrument types have been used in high-risk high-reward research initiatives and how frequently?</h3>

<img width="1102" height="553" alt="instrument_types" src="https://github.com/user-attachments/assets/324bc4e3-bb82-403d-a1a5-e3703febee83" />

Project grants for public research seem to be the most common policy instrument for high-risk high-reward initiatives, appearing in 56 different initiatives in the dataset. This is followed by strategies, agendas, and plans, which are used in 16 initiatives. Trailing slightly behind are grants for business R&D and innovation, which are used in 15 initiatives.

<h3>Question 3: What is the budget allocation for each policy instrument type used in high-risk high-reward research initiatives?</h3>

<img width="1083" height="536" alt="budget_allocation" src="https://github.com/user-attachments/assets/6536de7b-6f26-4218-8344-a8723852c879" />

Unsurprisingly, budget allocation follows a similar ranking to instrument types frequency mentioned above. Project grants for public research receive the highest overall funding, followed by strategies, agendas, and plans, and grants for business R&D and innovation.

As we are interested in funding for each instrument type but we only have the overall funding for the initiative, which can involve multiple instrument types, we split the funding unit equally between the instruments types used for the initiative. For example, if an initiative uses four instrument types, each is credited with 0.25 (25%) of the allocated budget for the initiative. This explains why some of the final counts include decimal values. It is acknowledged that this is not a perfect measure as some instruments type may have received more or less money than other instrument types in the initiative.

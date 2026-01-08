---
title: "What Ghana’s State of the Nation Addresses (SONA) Reveal About Politics, Policy, and Priorities: A Text Analytics Study" 
tech: R, Text analytics
featured: true
excerpt: >
    Text analytics provides a useful lens for understanding how presidents frame national priorities, justify policy choices, and communicate intent...
---  

## Findings and Data Overview  
This study analyzes Ghana’s State of the Nation Addresses (SONA) from 2001 to 2024 using text analytics techniques. Table 1 summarizes the documents used, showing the number of sentences and tokens for each year.
The year 2014 recorded the longest address, with 930 sentences and 23,929 tokens, closely followed by 2016, which had 900 sentences and 23,024 tokens. Shorter addresses, such as 2019, contained fewer sentences and tokens, indicating more concise speeches. Overall, the variation in document length suggests differences in governing priorities, economic conditions, and political context across administrations.   
Table 1: Summary of Documents  
| Year | Sentences | Tokens |
|------|-----------|--------|
| 2001 | 204 | 5115 |
| 2002 | 415 | 9591 |
| 2003 | 268 | 7031 |
| 2004 | 245 | 6787 |
| 2005 | 222 | 5458 |
| 2006 | 199 | 4945 |
| 2007 | 295 | 7373 |
| 2008 | 302 | 7212 |
| 2009 | 298 | 8072 |
| 2010 | 204 | 5618 |
| 2011 | 240 | 6676 |
| 2012 | 264 | 7435 |
| 2013 | 456 | 12354 |
| 2014 | 930 | 23929 |
| 2015 | 745 | 19484 |
| 2016 | 900 | 23024 |
| 2017 | 300 | 7255 |
| 2018 | 350 | 9435 |
| 2019 | 161 | 4801 |
| 2020 | 403 | 12063 |
| 2021 | 306 | 9158 |
| 2022 | 214 | 6289 |
| 2023 | 308 | 9928 |
| 2024 | 435 | 13648 |

### Most Frequent Words in SONA
![Top 20 most frequent words from SONA](/assets/images/Top%2020%20most%20freq%20words.png)  
 The bar chart of the top 20 most frequent words shows that “Ghana” and “government” appear most often. This is expected, as the speeches focus on presenting the state of Ghana and government actions to Parliament.
Other frequently used words include development, people, nation, education, economy, programme, and health. These words suggest that SONA speeches consistently emphasize national development, public welfare, and economic management.


![Top 20 words by term frequency-inverse document frequency](/assets/images/Top%2020%20IDF.png)  
### TF-IDF Analysis: What Makes Each SONA Distinct
The TF-IDF analysis highlights words that are more specific to particular addresses rather than common across all speeches. Financial and economic terms such as hundred, thousand, GHC, and IMF indicate strong attention to fiscal issues, public debt, and international financial engagement. Infrastructure-related words like roads, feeders, bitumen, and mining point to recurring discussions on road construction and natural resource development.
Education appears through terms such as TVET (Technical and Vocational Education and Training), suggesting a focus on skills development and employment. Health and social concerns are reflected in words like drugs and COVID, with COVID-19 clearly capturing the period of the global pandemic. Some words signal policy intent rather than completed action. Terms such as shall, raising, and PSI (President’s Special Initiative) indicate future commitments and planned interventions.  
Overall, the TF-IDF results show that SONA speeches place strong emphasis on economic recovery, infrastructure development, human capital, and crisis response, depending on the political and economic context of the time.  


### How Language Changes Across Political Transitions
#### The 2001 Transition to Civilian Rule
![Top 20 words in 2001](/assets/images/Top%20terms%20for%202001.png)
The 2001 SONA marked the beginning of structured State of the Nation Addresses under a constitutionally elected civilian government. Words such as shall, goal, and promise suggest a strong focus on future commitments and building public trust.  
Economic terms like debt, budget, and currency reflect concerns about the state of the economy at the start of the new administration. Governance-related words such as act, democracy, and right highlight efforts to strengthen democratic institutions and human rights after years of military rule.

![](/assets/images/Top%20words%20for%202009.png)
#### The 2009 Change of Government
In 2009, power transitioned from one democratically elected party to an opposition party. The prominence of words like debt and budget suggests concerns about inherited economic conditions. Terms such as enforce and act point to an emphasis on implementing laws and strengthening regulation. Words like review and aim indicate reassessment of existing policies to align with the new administration’s priorities. Infrastructure (road, transport) and social inclusion (women) also feature prominently, reflecting policy attention to development and gender-related issues.

In 2009, the democratically elected government of one party transitioned to a democratically elected government of an opposition party. Debt, budget, indicates concerns about public debt levels inherited from the outgoing administration. They highlight the importance of presenting a financial plan to address national priorities, allocate resources efficiently, and tackle economic challenges.  

![Top 20 words in 2017](/assets/images/Top%2020%20terms%20for%202017.png)
The 2017 Political Transition
The 2017 SONA followed another transition, this time from the NDC to the NPP. Economic terms such as debt, fiscal, GDP, and billion dominate, highlighting fiscal challenges and economic ambitions.  
Words like elect and change emphasize political transition and public expectations. Shall again signals policy promises, while food points to agricultural and food security concerns. The term force likely reflects efforts to strengthen institutions, law enforcement, or national security.

Topic Modelling in SONA

| Year | Topic |
|------|-------|
| 2001 | 3 |
| 2002 | 3 |
| 2003 | 2 |
| 2004 | 3 |
| 2005 | 2 |
| 2006 | 2 |
| 2009 | 2 |
| 2010 | 3 |
| 2011 | 3 |
| 2012 | 2 |
| 2013 | 2 |
| 2014 | 5 |
| 2015 | 5 |
| 2016 | 5 |
| 2017 | 3 |
| 2018 | 1 |
| 2019 | 1 |
| 2020 | 3 |
| 2021 | 4 |
| 2022 | 4 |
| 2023 | 4 |
| 2024 | 4 |


| Topic 1 | Topic 2 | Topic 3 | Topic 4 | Topic 5 |
|--------|--------|--------|--------|--------|
| year | govern | govern | ghana | road |
| govern | nation | year | year | ghana |
| countri | ghana | nation | countri | year |
| ghana | develop | ghana | hundred | work |
| hundred | year | countri | one | nation |
| one | sector | peopl | govern | region |
| make | countri | state | nation | project |
| nation | privat | sector | project | govern |
| hous | educ | develop | construct | peopl |
| develop | work | work | three | educ |



### Topic Modelling Results
Using Latent Dirichlet Allocation (LDA), five main topics were identified across the SONA documents. These topics broadly relate to:
- Governance and national identity
- Economic development and infrastructure
- Education and human capital
- Public sector projects and implementation
- Social and regional development
The distribution of topics varies by year, suggesting that presidential focus shifts depending on political transitions, economic pressures, and national challenges.

### Sentiment Analysis
![Sentiment Analysis by Document](/assets/images/Sentiment%20analysis%20per%20document.png)

Across all years, SONA speeches exhibit more positive than negative sentiment. Longer speeches tend to contain more positive and negative sentiment simply because they include more content.  
Years such as 2014 and 2016, which had the longest addresses, recorded the highest levels of both positive and negative sentiment. In contrast, 2019, which had the shortest address, showed the lowest sentiment counts.
This suggests that sentiment levels are influenced more by speech length than by sharp changes in tone.

Conclusion
This analysis shows that Ghana’s State of the Nation Addresses reflect both continuity and change in political communication. While development, governance, and economic management remain consistent themes, specific word choices shift with political transitions, economic conditions, and national crises.
Text analytics provides a useful lens for understanding how presidents frame national priorities, justify policy choices, and communicate intent. Rather than relying on anecdotal impressions, this approach offers empirical evidence of how political language evolves over time in Ghana’s democratic context.


## I-AID: Identifying Actionable Information from Disaster-related Tweets
This repository contains the source-code and datasets of the I-AID approach discussed in:
[I-AID: Identifying Actionable Information from Disaster-related Tweets](https://arxiv.org/abs/2008.13544). By ```Hamada M. Zahera, Rricha Jalota, Mohamed A. Sherif and Axel N.Ngnoga (DICE group, Department of Computer Science, Paderborn University)```

## Summary: 
Social media plays a significant role in disaster management by providing valuable data about affected people, donations, and help requests. Recent studies highlight the need to filter information on social media into fine-grained content labels. However, identifying useful information from massive amounts of social media posts during a crisis is a challenging task. In this paper, we propose I-AID, a multimodel approach to automatically categorize tweets into multi-label information types and filter critical information from the enormous volume of social media data. I-AID incorporates three main components: 
i) a BERT-based encoder to capture the semantics of a tweet and represent as a low-dimensional vector, ii) a graph attention network (GAT) to apprehend correlations between tweets' words/entities and the corresponding information types, and iii) a Relation Network as a learnable distance metric to compute the similarity between tweets and their corresponding information types in a supervised way. We conducted several experiments on two real publicly available datasets. Our results indicate that I-AID outperforms state-of-the-art approaches in terms of weighted average F1 score by +6% and +4% on the TREC-IS dataset and COVID-19 Tweets, respectively. 

---

## Dependencies:

```
python 3.6
tensorflow 2.0
spaCy 3.0
NLTK 3.6.2 
scikit-learn 0.24
pickle5 0.0.11
```
## Installation:
You can install all requirements via: ```pip install -r requirements.txt```
## Dataset:
We conducted our experiments on two public datasets provided by TREC (TREC-IS 2019 edition and COVID-19 Tweets):
- <b>TREC-IS</b>: this dataset contains approximately 35K tweets collected during 33 different disasters between 2012 and 2019 (e.g., wildfires, earthquakes, hurricanes, bombings,} and floods). The tweets are labeled with 25 information types by human experts and volunteers. 
    
- <b>COVID-19 Tweets</b>:  this dataset contains a collection of tweets about the COVID-19 outbreak in different affected regions. In total, the data has 7,5k tweets labeled with one or more of the full 12 information type labels (the same as for the TREC-IS dataset). 
## Run the code:
We provide descriptive notebooks for our approach and baseline methods in ```notebook``` folder. We share also our implementation publicly on ```Google colab``` server.  

---
## Cite: 
```
Hamada M. Zahera, Rricha Jalota, Mohamed A. Sherif and Axel N.Ngnoga (DICE group, Department of Computer Science, Paderborn University)
```
## Contact:
If you have any further questions/feedback, please contact corresponding author at [hamada.zahera@uni-paderborn.de](mailto:hamada.zahera@uni-paderborn.de)


# DATA 512 A1: Data Curation
## Goals:
The goal of this assignment is to identify what, if any, sources of bias may exist in these datasets, and to develop testable hypotheses about how these biases might impact the behavior of machine learning models trained on the data, when those models are used for research purposes or to power data-driven applications. 

Overview of the research project : https://meta.wikimedia.org/wiki/Research:Detox

Perspective API on GitHub: https://github.com/conversationai/perspectiveapi/blob/master/2-api/methods.md


## Data Source:
The corpus we used is called the Wikipedia Talk corpus, and it consists of three datasets. Each dataset contains thousands of online discussion posts made by Wikipedia editors who were discussing how to write and edit Wikipedia articles. Crowdworkers labelled these posts for three kinds of hostile speech: “toxicity”, “aggression”, and “personal attacks”. Many posts in each dataset were labelled by multiple crowdworkers for each type of hostile speech, to improve accuracy.
Liscence : [MIT](https://github.com/ankitapal189/data-512/blob/main/data-512-a1/LICENSE.md)<BR>
Terms of Use : https://www.mediawiki.org/wiki/Wikimedia_REST_API#Terms_and_conditions<BR>
 <BR>
 We used 2 Daatsets:<BR>
    1. Wulczyn, Ellery; Thain, Nithum; Dixon, Lucas (2017): Wikipedia Talk Labels: Personal Attacks. figshare. Dataset. https://doi.org/10.6084/m9.figshare.4054689.v6<BR>
  2.Thain, Nithum; Dixon, Lucas; Wulczyn, Ellery (2017): Wikipedia Talk Labels: Toxicity. figshare. Dataset. https://doi.org/10.6084/m9.figshare.4563973.v2

## Research questions and Results:
#### **1. Analyze the demographic information about the Crowdflower workers that is available in the dataset and how it fits the real world population.**

There is a bias in age and education that reflects the general population. There is a gender bias that does not represent the general population.

#### **2. Explore relationships between worker demographics and labeling behavior.**

Gender, education and age does not create a bias on the toxicity and personal attack flag.

## Outputs:
| Image | Description |
|--------|-------------|
| Age_group_demographics.png | Comparison of populations in each age group |
| Education_demographics.png |  Comparison of populations having various levels of education |			
| Gender_demographics.png |  Comparison of populations belonging to each gender  |
| Personal_attack_age_group.png | The age group distribution of the population who flagged comment to be a personal attack |
| Personal_attack_education_levels.png | The education level distribution of the population who flagged comment to be a personal attack |
| Personal_attack_gender.png |  The gender distribution of the population who flagged comment to be a personal attack   |
| Toxicity_age_group.png | The age group distribution of the population who flagged comment to be toxic |
| Toxicity_education_levels.png | The education level distribution of the population who flagged comment to be toxic |
| Toxicity_gender.png |  The gender distribution of the population who flagged comment to be toxic   |

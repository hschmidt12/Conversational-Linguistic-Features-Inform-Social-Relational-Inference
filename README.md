This project includes data and code for the following paper:

**Schmidt, H., Tran, S., Medaglia, J.A., Ulichney, V., & Helion, C. (2022). Conversational linguistic features predict social network learning.**

Additional information can be found on OSF at: https://osf.io/8wqhb/

# Abstract
Whether it is the first day of school or a new job, individuals often find themselves in situations where they must quickly and accurately learn novel social networks. Prior work has shown that success in learning social networks predicts more positive individual and social outcomes, but the mechanisms through which social network learning occurs are unclear. We posit that individuals use linguistic features of observed conversations to identify the valence and strength of social relationships. To investigate this, 57 adults completed a naturalistic behavioral task wherein they watched an episode of the reality television show, Survivor, and indicated which contestants they thought were friends or rivals throughout the episode. In Study 1, we take a person-focused approach using 34,735 participant observations to understand how well individuals learned the social network structure. In Study 2, we take a novel stimulus-focused approach that employs natural language processing to quantify 486 sentences of episode dialogue and examine how distinct linguistic features (similarity, emotional tone, self-assurance) predict network learning. In Study 3, we analyze the time course of the entire preceding season of Survivor using 296 dyadic similarity assessments to explore the association between semantic similarity and relationship formation. Across three studies, we found that participants successfully learned the social network structure, linguistic features predicted network learning, and greater semantic similarity was associated with friendship formation. These findings suggest that naturalistic conversational content is both a potential mechanism of social network learning and a promising avenue for research on social relational inference.

# Data

The `data` folder contains all de-identified data using in this paper. 

 - `dat_survivor.csv` contains raw participant-level responses
 - `df-clean.csv` contains all raw participant-level responses merged with NLP linguistic scores (similarity, sentiment, clout)
 - `df-ling.csv` contains raw participant-level responses merged with NLP linguistic scores, but only contains trials that have corresponding linguistic data
 - `friends-dyads.csv` contains data on how often each contestant pair (dyad) was chosen as friends
 - `friends_rivals_dyads.csv` contains data on how often each dyad was chosen as friends and rivals
 - `LIWC_clout.csv` contains output from LIWC with clout scores per sentence of contestant dialogue
 - `rival-dyads.csv` contains data on how often each dyad was chosen as rivals
 - `similarity_choices.csv` contains data on participant-level responses merged with similarity scores
 - `Similarity-data.csv` contains reformatted similarity scores for all episode clips (created from the clip-specific similarity matrices)
 - `survivor-split-sentences.csv` contains all contestant dialogue from the episode with each row containing one sentence of dialogue; each row is labeled with the word count in that sentence
 - `survivor-text.csv` contains raw contestant dialogue from the episode with each row containing one sentence of dialogue 

Within the `data` folder, there is a subfolder called `clips` that contains the clip-specific semantic similarity matrices (6 .csv files).

# Scripts

All scripts associated with this paper are included here. These scripts are formatted as R Markdowns and each script has a corresponding .html file. 

 1. `Data-Cleaning-and-Setup` - Reads in raw response data and formats it for NLP analyses
 2. `Study1-Network-Discernment` - Runs five analyses to assess if participants successfully learned the social network of the episode
 3. `Study2-Linguistic-Features` - Runs three multilevel linear regressions to assess to what extent each linguistic feature predicts relationship judgments
 4. `Study3-Similarity-Over-Time` - Runs a multilevel linear regression to assess how relationship judgments at the time of evaluation predict earlier levels of semantic similarity

Please direct any comments or questions to Helen Schmidt at helen_schmidt@temple.edu. Please feel free to use any of these scripts, but unfortunately I am unable to provide support if you adapt them to your own data. If you notice a bug or error, please tell me! 


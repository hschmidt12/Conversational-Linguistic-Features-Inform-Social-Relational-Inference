This project includes data and analytic scripts for the following paper:

**Schmidt, H., Tran, S., Medaglia, J.A., Ulichney, V., Mitchell, W.J., & Helion, C. (under review). Conversational Linguistic Features Inform Social-Relational Inference. *PsyArXiv Pre-Print: https://psyarxiv.com/fn4my/***

Additional information can be found on OSF at: https://osf.io/8wqhb/

# Abstract

*Coming soon*

# Data

The `data` folder contains all de-identified data. 

 - `dat_survivor.csv` contains raw participant-level responses
 - `survivor-text.csv` contains raw contestant dialogue from the episode with each row containing one sentence of dialogue 

# Scripts

All scripts associated with this project are included. Analyses were performed in R and Python: R scripts are formatted as .qmd files and Python scripts are formatted as .ipynb files. R analytic scripts are numbered for reproducibility. Clout scores are calculated using the Linguistic Inquiry and Word Count (LIWC) software, semantic similarity is calculated using the Universal Sentence Encoder (4) in Python, and sentiment is calculated using the `sentimentr` package in R. 

 1. `1-data-cleaning-and-setup` - Loads raw task data, calculates sentiment scores, loads similarity (see USE subfolder) and clout scores, combines all data
 2. `2-rsa-behavioral` - Examines task response similarity across participants using representational similarity analysis (RSA)
 3. `3-bayesian-clout-modeling` - Fits Bayesian statistical models to examine association between social-relational inference and conversational clout
 4. `3-bayesian-sentiment-modeling` - Fits Bayesian statisical models to examine association between social-relational inference and conversational sentiment
 5. `3-bayesian-similarity-modeling` - Fits Bayesian statistical models to examine association between social-relational inference and conversational semantic similarity
 6. `4-all-features-modeling` - Fits LASSO regression model to examine overlapping contributions of all three conversational linguistic features
 7. `5-whole-season-transcription-wrangling` - Formats transcriptions for first five episodes in the *Survivor* season
 8. `6-whole-season-bayesian-similarity-modeling` - Fits Bayesian statistical models to examine association between early semantic similarity and later social-relational inference
 9. `7-supplemental` - Creates some supplemental plots (others are created in earlier scripts)
 10. `8-extract-posterior-draws` - Extract posteriors from Bayesian models and create plots

Please direct any comments or questions to Helen Schmidt at helen_schmidt@temple.edu. Please feel free to use any of these scripts, but unfortunately I am unable to provide support if you adapt them to your own data. If you notice a bug or error, please tell me! 


# SDS 384 Team 9
## Classification of plant-associated bacteria based on genome features
*Repo for scripts and documentation for classifier of plant associated and non-plant associated bacteria*

## Rationale and Goals for this project
Recent publications exploring genomes in broad phyla [Levy et. al., 2017](https://www.nature.com/articles/s41588-017-0012-9), and within a focused genus [Santamaria et. al., 2022](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9769992/), suggest that the presence of carbohydrate associated genes is correlated with plant association in many bacterial phyla. Identifying a core bacterial population associated with plants or novel bacterial/plant clusters could greatly accelerate metabolic engineering and synthetic biology approaches to engineer the plant rhizosphere, which has agricultural applications. 

We hypothesize that machine learning and bioinformatics tools can be used to predict if a new bacteria is plant or non-plant associated (PA, NPA, respectively). This is a binary classification problem. The features used to train the model include taxonomy information, presence of carbohydrate associated genes in the available genome sequences (identified by [dbCAN4](https://github.com/linnabrown/run_dbcan)) and an existing dataset describing the isolation source of many bacterial species as well as many other features. Models such as Random Forest classification and an Ensemble Model will be trained on the data. The goal is to develop a successful model with an F1 score above 0.7.

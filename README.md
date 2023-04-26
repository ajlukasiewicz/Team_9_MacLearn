# SDS 384 Team 9
## Classification of plant-associated bacteria based on genome features
*Repo for scripts and documentation for classifier of plant associated and non-plant associated bacteria*

## Rationale and Goals for this project
Recent publications exploring genomes in broad phyla [Levy et. al., 2017](https://www.nature.com/articles/s41588-017-0012-9), and within a focused genus [Santamaria et. al., 2022](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9769992/), suggest that the presence of carbohydrate associated genes is correlated with plant association in many bacterial phyla. Identifying a core bacterial population associated with plants or novel bacterial/plant clusters could greatly accelerate metabolic engineering and synthetic biology approaches to engineer the plant rhizosphere, which has agricultural applications. 

We hypothesize that machine learning and bioinformatics tools can be used to predict if a new bacteria is plant or non-plant associated (PA, NPA, respectively). This is a binary classification problem. The features used to train the model described herein include the presence of carbohydrate-associated enzymes and COGs (Clusters of Orthologous Genes) in the available genome sequences as well as the horizontal gene transfer of each genome. This totals approximately 4,000 features. The total number of genomes is over 3,000, approximately an order of magnitude greater than Martínez-García et al., 2016. Supervised learning models, including Random Forest classification, K-nearest neighbors, XGBoost Classifier, and Logistic Regression, were trained on the data. 

## Scripts
This main branch includes the script after the feacture selection using merged features. Each one's branch has script for data processing and feature selection.

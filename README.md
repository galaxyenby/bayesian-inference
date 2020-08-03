# Generative Classifier applied to Health Data
This project is primarily about using Generative density models (examples: Gaussian Mixture model, Kernel Density model) in the context of Bayesian Inference to predict carcinoma in the Hepatocellular Carcinoma (HCC) patients database collected by the University of Madrid.  I'm working specifically with this dataset since it only contains 165 patient-records, so it's a fairly small dataset (typical of medical datasets) to apply typical machine learning predictive models such as logistic regression & neural networks.

BIG EDIT: I was able to re-train the density estimation models WITHOUT having to re-sample and class-balance, so gaussian mixture with "tied" distribution is a huge improvement (especially in false-positive-rate) over logistic regression with a training size of ~100 records.

I'll be using the hcc-dataset.csv provided on Kaggle by Miriam Santos, the author of this particular work on applying a new nearest-neighbor approach to fill in missing data. The HCC dataset will be in this repo as well.

I've written two Medium articles outlining my thinking process on this project: 
1. https://medium.com/swlh/explainable-ai-where-supervised-learning-can-falter-edf2b562845a
2. https://towardsdatascience.com/explainable-ai-use-case-1-bc2abd7b197a

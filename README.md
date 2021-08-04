# RandomForestsForPredictingUnitCellProperties

A repository for the machine learning associated with the paper "Chemically controllable magnetic transition temperature and magneto-elastic coupling in MnZnSb compounds"

## Data

Data is preprocessed and split into three datasets for experimentation as specified in the supplimentary information of the paper:

* ICSD - all compounds in the inorganic crystal database as of 2018.
* ICSDandMP - a union of experimentally measured structures in the ICSD and Density Functional Theory (DFT) measured structures with a Tetragonal symetry in the Materials Project
* PbFCl - All PbFCl type structures in Pearson's Crystal Database

Each dataset has a subfolder in the Data directory, in each subfolder you can find:

* The dataset in full
* The dataset marked with is_train to denote the train/test split used in the paper
* The dataset as paired for use in the substitional predictions
* Leave one cluster out cross validation splits (for k = 2 to k=10) for both the paired and normal versions of this dataset

## Machine Learning Code

This code predicts a veriety of unit cell lattice parameters from composition. Predictions are made either as a regressor or through ordinal classification as discussed in the associated paper. Ordinal classification is helpful for substituional studies. For example one might ask "if I replace Manganese with Chromium in my compound will the C:A ratio get larger or smaller?" this resulted in more accurate predictions, though it does require knowledge of lattice parameters in the original compound. This is useful where the affect of a phenomena is associated with lattice parameters for example magneto calorics in the PbFCl family (as discussed in the associated paper), however this concept could be applied more broadly to any property prediction problem that will be investigated with substituional study

Two ipynb files have been uploaded:
* FindShannonRadius.ipynb takes you through the deffinition we use for Shannon radius (we use weighted shannon radius as a naive benchmark in our work)
* MachineLearningForLatticeParamaters takes you through prediction types for the example property c/a ratio, on the PbFCl dataset, variables are listed near the top of the file should you want to change it to use this code to predict a different unit cell lattice parameter

## Citations:
If you find this repository helpful please cite the associated paper:
@article{Murgatroyd2021,
author = {Murgatroyd, Philip A. E. and Routledge, Kieran and Durdy, Samantha and Gaultois, Michael W. and Surta, T. Wesley and Dyer, Matthew S. and Claridge, John B. and Savvin, Stanislav N. and Pelloquin, Denis and H{\'{e}}bert, Sylvie and Alaria, Jonathan},
doi = {10.1002/adfm.202100108},
issn = {1616-301X},
journal = {Advanced Functional Materials},
keywords = {chemical control,computational proxy,machine learning,magnetic materials,magnetocalorics},
month = {apr},
number = {17},
pages = {2100108},
publisher = {John Wiley and Sons Inc},
title = {{Chemically Controllable Magnetic Transition Temperature and Magneto‐Elastic Coupling in MnZnSb Compounds}},
url = {https://onlinelibrary.wiley.com/doi/10.1002/adfm.202100108},
volume = {31},
year = {2021}
}

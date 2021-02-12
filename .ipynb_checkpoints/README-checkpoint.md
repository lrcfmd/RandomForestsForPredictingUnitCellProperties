# RandomForestsForPredictingUnitCellProperties

A repository for the machine learning associated with the paper "Chemically controllable magnetic transition temperature and magneto-elastic coupling in MnZnSb compounds"

## Data

Data is preprocessed and split into three datasets for experimentation as specified in the supplimentary information of the paper:

* ICSD - all compounds in the inorganic crystal database as of 2018.
* ICSDandMP - a union of experimentally measured structures in the ICSD and Density Functional Theory (DFT) measured structures with a Tetragonal symetry in the Materials Project
* PbFCl - All PbFCl type structures in Pearson's Crystal Database

Each dataset has a subfolder in the Data directory, in each subfolder you can find:

* The dataset in full
* The dataset market with is_train to denote the train/test split used in the paper
* The dataset as paired for use in the substitional predictions
* Leave one cluster out cross validation splits (for k = 2 to k=10) for both the paired and normal versions of this dataset


## Citations:
If you find this repository helpful please cite the associated paper:

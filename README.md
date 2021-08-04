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

## Machine Learning Code

To be uploaded. This code predicts a veriety of unit cell lattice parameters from composition. Predictions are made either as a regressor or through ordinal classification as discussed in the associated paper. Ordinal classification is helpful for substituional studies. For example one might ask "if I replace Manganese with Chromium in my compound will the C:A ratio get larger or smaller?" this resulted in more accurate predictions, though it does require knowledge of lattice parameters in the original compound. This is useful where the affect of a phenomena is associated with lattice parameters for example magneto calorics in the PbFCl family (as discussed in the associated paper), however this concept could be applied more broadly to any property prediction problem that will be investigated with substituional study

## Citations:
If you find this repository helpful please cite the associated paper:
@article{Murgatroyd2021,
<<<<<<< HEAD
abstract = {Magneto-caloric materials offer the possibility to design environmentally friendlier thermal management devices compared to the widely used gas-based systems. The challenges to develop this solid-state based technology lie in the difficulty of finding materials presenting a large magneto-caloric effect over a broad temperature span together with suitable secondary application parameters such as low heat capacity and high thermal conductivity. A series of compounds derived from the PbFCl structure is investigated using a combination of computational and experimental methods focusing on the change of cell volume in magnetic and non-magnetic ground states. Scaling analysis of the magnetic properties determines that they are second order phase transition ferromagnets and that the magnetic entropy change is driven by the coupling of magneto-elastic strain in the square-net through the magnetic transition determined from neutron and synchrotron X-ray diffraction. The primary and secondary application related properties are measured experimentally, and the c/a parameter is identified as an accurate proxy to control the magnetic transition. Chemical substitution on the square-net affords tuning of the Curie temperature over a broad temperature span between 252 and 322 K. A predictive machine learning model for the c/a parameter is developed to guide future exploratory synthesis.},
=======
>>>>>>> b21ee3578ccb22bd8145620b697b7113e4bfa885
author = {Murgatroyd, Philip A. E. and Routledge, Kieran and Durdy, Samantha and Gaultois, Michael W. and Surta, T. Wesley and Dyer, Matthew S. and Claridge, John B. and Savvin, Stanislav N. and Pelloquin, Denis and H{\'{e}}bert, Sylvie and Alaria, Jonathan},
doi = {10.1002/adfm.202100108},
issn = {1616-301X},
journal = {Advanced Functional Materials},
keywords = {chemical control,computational proxy,machine learning,magnetic materials,magnetocalorics},
<<<<<<< HEAD
month = {apr},
number = {17},
pages = {2100108},
publisher = {John Wiley and Sons Inc},
title = {{Chemically Controllable Magnetic Transition Temperature and Magneto‐Elastic Coupling in MnZnSb Compounds}},
url = {https://onlinelibrary.wiley.com/doi/10.1002/adfm.202100108},
volume = {31},
year = {2021}
}
=======
month = {feb},
pages = {2100108},
publisher = {John Wiley & Sons, Ltd},
title = {{Chemically Controllable Magnetic Transition Temperature and Magneto‐Elastic Coupling in MnZnSb Compounds}},
url = {https://onlinelibrary.wiley.com/doi/10.1002/adfm.202100108},
year = {2021}
}

>>>>>>> b21ee3578ccb22bd8145620b697b7113e4bfa885

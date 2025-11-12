# mobo-medium-conditions
This repository contains the code and data for "Optimal medium condition design with Bayesian methods".

## Folder Structure
* **Analysis** -
  Contains the jupyter notebooks with the code used to generate the figures used in the publication as well as for the supplementary figures.
* **Data** -  
  Contains the data used to to generate the figures used in the publication as well as for the supplementary figures.
* **figs** -
  Contains the figures used in the publication as well the supplementary figures.
* **optimization** -
  Contains the complete code to run the simulations and verify the results.

## Adapting the Method to Your Project
Currently, it is possible to optimise for any combination of growth (biomass vector), production (of one compound of interest, given by production flux), and medium cost.
To adapt it to your model, you should only have to work in Main_MOBO.ipynb
* you need to load your model (and potentially modify it so that it fits the naming conventions of CobraPy)
* define the medium components, their bounds, and their costs (default values will be chosen of they are not defined)
* pass the desired parameters to the function `media_BayesOpt`

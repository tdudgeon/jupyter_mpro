# Jupyter notebooks for playing with Mpro virtual screening info

This notebook is a collection of examples for processing the MPro fragment screening virutal screening follow up data.

This is not supposed to be the definitive way to approach this, just a collection of suggestions.

See these links for background on the project:
- https://www.diamond.ac.uk/covid-19/for-scientists/Main-protease-structure-and-XChem.html
- https://covid19.galaxyproject.org/cheminformatics

If running a local Jupyter environment create a conda environment:

```
conda env create -f environment.yml
```

Then activate the environment:
```
conda activate jupyter-xchem
```

Then start Jupyter:
```
jupyter notebook
```

## Notebooks

The following notebooks may be of interest:

- [Score_distrbutions.ipynb](Score_distrbutions.ipynb) - initial playground with a hotch-potch of appraoches that are used in the main notebooks.
- [1_DataPrep.ipynb]() - initial data merging and preparation.
- [2_InititalDataAnalysis.ipynb](1_DataPrep.ipynb]) - basic analysis of the results.
- [3_AugmentationAndFiltering.ipynb](3_AugmentationAndFiltering.ipynb) - augmentation and filtering of the results.


## Datasets

The following datasets may be of interest: 

1. Mpro_16_data.sdf.gz -  SD file containing the output of the 1_DataPrep notebook
2. Mpro_16_data.smi.gz - file with the SMILES from the output from the 1_DataPrep notebook
3. Enalos_data.csv.gz - ADMET data provided by NovaMechanics Ltd through Enalos Suite that is used in the 3_AugmentationAndFiltering notebook

If you are wanting to generate data that can be used in the process of selecting compounds (see the Enalos data as
an example) you should use datasets 1 or 2 and PLEASE make sure the SMILES string (title line of the SDF) is included in
your data so that it can be merged into the main data.

## Updates

This data is continually being updated. We try to keep this README up to date.
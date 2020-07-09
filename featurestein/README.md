# FeatureStein

FeatureStein uses merged RDKit feature maps to determine the overlap of a ligand pose with an ensemble of fragment hits.
It genreates a score between 0 and 1 (occsaionally slightly greater than one) with 0 meaning no overalp and 1 maning perfect
overlap. The overlap is based on the RDKit feature maps.

## Methodology

This contained in the [FeatureStein.ipynb]() notebook.
It allows the 23 non-covalent or the 69 covalent and non-covalent Mpro fragment hits to be built into a merged feature map
that is saved as a Python pickle.

## Scoring

### FragmentStein scoring

Matteo Ferla's FragmentStein ligands are scored with Featurestein in the [ScoreFragmentsteinLigands.ipynb]() notebook
This notebook runs in a few minutes.
A file in the format for upload to Fraglysis is generated.

### Galaxy Gen3 XChem virtual screening workflow scoring

The poses from the Generation 3 fragment screening follow up workflow are scored with Featurestein in the [ScoreGalaxyGen3Ligands.ipynb]() notebook. 
This notebook can take several hours to run depending on how many top scoring poses are retained.
A SDF file is generated for further analysis.

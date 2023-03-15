# geneGPT

## Data required:

* [`AML_datasets.RData`](https://uni-bonn.sciebo.de/s/Uiv84S0XR9XLuch) - initial dataset as provided by paper
* `gene.RData` - created when running the `genesignature.ipynb` notebook
* `data.RData` - created when running the `splitdata.ipynb` notebook
## How to run

1. Ensure `AML_datasets.RData` is in project directory. 

The datasets created are too big to be committed to the repository, and thus the feature selection and data split is left to be created by the user.

2. Run `genesignature.ipynb` notebook to generate `gene.RData.` This creates the list of gene signatures to train the models using the feature selection method proposed in the paper
3. Run `splitdata.ipynb` notebook to generate `data.RData`. This creates the train/test splits for the models to use for training.
4. Run `models.ipynb`. This trains the models first using the gene signatures selected via the proposed method in the paper, then by using the alternative gene signatures as proposed by group Genome Seeker, and finally cross validation is performed using the first set of gene signatures

# geneGPT

## Data required:
*Note: access to team discord required*
* [`gene.RData`](https://discord.com/channels/1075285485716512849/1075468562170400948/1085336148903202879)
* [`data.RData`](https://discord.com/channels/1075285485716512849/1075468562170400948/1085336357284626482)
* [`AML_datasets.RData`](https://uni-bonn.sciebo.de/s/Uiv84S0XR9XLuch)
* `alternate_genesig.txt`

Order to run notebook:
1. splitdata.ipynb (need AML_datasets.RData)
  
      *This notebook will produce data.RData*

2. genesignature.ipynb (need data.RData)
  
      *This notebook will produce gene.RData*

3. models.ipynb (need AML_datasets.RData, data.RData, and gene.RData)

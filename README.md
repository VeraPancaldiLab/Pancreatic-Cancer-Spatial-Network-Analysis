# **PNETS-NETS**
## **Pancreatic Cancer Network Reconstruction and Analysis**

This repository use *mosna* and *tysserand* packages 

### Tysserand
[tysserand](https://github.com/VeraPancaldiLab/tysserand) is a Python library to reconstruct spatial networks from spatially resolved omics experiments. It is intended as a common tool where the bioinformatics community can add new methods to reconstruct networks, choose appropriate parameters, clean resulting networks and pipe data to other libraries.
You can find the article and supplementary information on [Bioinformatics](https://academic.oup.com/bioinformatics/article-abstract/37/21/3989/6313163?redirectedFrom=fulltext), and the freely available preprint is on [BioRxiv](https://www.biorxiv.org/content/10.1101/2020.11.16.385377v1.full).

### Mosna (Multi-Omic Spatial Network Analysis)
[Mosna](https://github.com/AlexCoul/mosna) is an in-devlopement python package to find patterns and communities in spatial networks of nodes with attributes of possibly high dimension.


### Create and activate environement using *conda*

~~~
# create env
conda env create -f conda_env_spatial-networks.yml

# activate/change env
conda activate spatial-networks

#list installed packages in env
conda list
~~~


### Workflow steps

1. Extract csv from fcs files
2. Extract jpg from CZI image
3. Compute nodes (nuclei) and their connections (edges) *[Tysserand]*
4. Cluster by markers (CDx, Mx, Cancer...)
5. Compute Mixing Matrix *[Mosna]*

![Workflow](/Figures/workflow1.png)



### Expected outputs
1. Cell coordinate files (csv)
2. JPG/PNG files extracted from CZI
3. Network nodes (csv)
4. Network vizualisation
5. Mixing matrix (csv and heatmap)



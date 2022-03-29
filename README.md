# **PNETS-NETS**
## **Pancreatic Cancer Network Reconstruction and Analysis**

### Packages
This repository use mosna and tysserand packages 

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
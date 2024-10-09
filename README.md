# PyG_Explore
This repo stores the notebooks and other resources related to the findings and implementations of PyG

# Setup

```
create a virtual environment

pip install -r requirements.txt

# uninstall torch and torch_geometric if the versions are not compatible with your environment (sometimes requires running the command twice)
pip uninstall torch_geometric
pip uninstall torch
pip uninstall torch

# install torch and torch_geometric by finding appropriate versions
# https://pytorch.org/get-started/locally/
# https://pytorch-geometric.readthedocs.io/en/latest/notes/installation.html

# now install jupyter notebook in the current virtualenv
pip install notebook

# install ipykernel and also register the specific kernel to this virtualenv (this enables using the notebook with the preferred virtualenv)
pip install ipykernel
python -m ipykernel install --user --name=<env_name>

# go to the project folder and run jupyter from there
cd ...path_to_Pyg_Explore/
jupyter notebook


```

# Projects

### GNN Hands on Part 1 

This notebook starts a hands on demonstration of the graph data and relevant concepts required for GNN tasks

### Splits

This notebook shows the study of Node vs Edge level splits in pyg. We study the methods RandomNodeSplit vs RandomLinkSplit on toy datasets. There is a load_file method which can load any pkl file. Our datasets are homogeneous and heterogeneous graphs. The code can be applied to any sort of dataset as long as it is a pyg graph.

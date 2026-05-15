This folder contains materials for the ChemProp and ChemTorch workshop by Esther Heid, at CAMLC 2026.

## Installation instructions part 2 (ChemTorch):

### Google Colab: 
Nothing, just click on `Workshop_ChemTorch_Demo_Jupyter.ipynb`, and then click the "Launch in Colab" button

### Own device:
To setup your environment: 
```
wget https://raw.githubusercontent.com/hesther/teaching/refs/heads/main/camlc2026/environment.yml
conda env create -f environment.yml  
conda activate chemtorch
git clone https://github.com/heid-lab/chemtorch.git
cd chemtorch
pip install rdkit numpy==1.26.4 scikit-learn pandas torch hydra-core wandb ipykernel jupyter matplotlib
pip install torch_geometric
pip install torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.10.0+cpu.html
pip install -e .
pip install chemprop
```
(if you would like to install with an accelerator, e.g. a gpu, specificy it instead of `cpu`, `cu128`, etc.
Then, download the notebook and start coding:
```
wget https://raw.githubusercontent.com/hesther/teaching/refs/heads/main/camlc2026/Workshop_ChemTorch_Demo_Jupyter.ipynb
jupyter notebook
```



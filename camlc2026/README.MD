This folder contains materials for the ChemProp and ChemTorch workshop by Esther Heid, at CAMLC 2026.

### Slides
Please see [2026_06_CAMLC.pdf](https://github.com/hesther/teaching/blob/main/camlc2026/2026_06_CAMLC.pdf) (you might need to download the file to see it depending on your browser, since PDF preview is not very stable on GitHub).

## Installation instructions:

### Google Colab: 
Just click on `Workshop_ChemTorch_Demo.ipynb`, and then click the "Launch in Colab" button (no installation required).

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



This folder contains materials for the ChemProp and ChemTorch workshop by Esther Heid, at CAMLC 2026.

## Installation instructions part 2 (ChemTorch):

### Google Colab: 
Nothing, just click on `Workshop_ChemTorch_Demo_Jupyter.ipynb`, and then click the "Launch in Colab" button

### Own device:
To setup your environment: 
```
git clone https://github.com/heid-lab/chemtorch.git
cd chemtorch
conda env create -f environment.yml  
conda activate chemtorch
uv sync --extra cpu && uv run scripts/install_pyg_deps.py --run   
conda install jupyter
```
(if you would like to install with an accelerator, e.g. a gpu, specificy it instead of `cpu`, e.g. `macos`, `cu128`, etc.
Then, download the notebook and start coding:
```
wget https://raw.githubusercontent.com/hesther/teaching/refs/heads/main/camlc2026/Workshop_ChemTorch_Demo_Jupyter.ipynb
jupyter notebook
```



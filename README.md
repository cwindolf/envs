# envs

Get mambaforge: https://github.com/conda-forge/miniforge

The below stuff only works with `mamba`, `conda` has trouble getting env `a` together.

```bash
mamba create -n jupy python=3.10 jupyterlab jupytext ipywidgets widgetsnbextension nodejs nb_conda_kernels python-lsp-server black pyright jupyterlab-lsp
mamba activate jupy
pip install jupyterlab-sublime jupyterlab-code-formatter
```

```bash
mamba create -n a python=3.10 numba seaborn scikit-learn scikit-image ipywidgets h5py colorcet tqdm joblib hdbscan cython matplotlib-venn
mamba activate a
# go to pytorch.org and find install instructions if you want gpu!
mamba install pytorch torchvision torchaudio -c pytorch
pip install ibllib
# -e install your local repositories
```

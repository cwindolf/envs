# envs

Get miniforge: https://github.com/conda-forge/miniforge

```bash
mamba create -n jupy python=3.13 jupyterlab ipywidgets ipykernel nb_conda_kernels seaborn jupytext ipython ipykernel widgetsnbextension nodejs jupyterlab-lsp basedpyright jedi-language-server ipympl
mamba activate jupy
```

```bash
mamba create -n a python=3.11 numba seaborn scikit-learn scikit-image ipywidgets h5py colorcet tqdm joblib hdbscan cython matplotlib-venn pyfftw
mamba activate a
# go to pytorch.org and find install instructions if you want gpu!
mamba install pytorch torchvision torchaudio -c pytorch
pip install ibllib
# pip -e install . your local repositories
```

I would recommend installing spikeinterface, probeinterface, and neo locally from their git repos: https://github.com/SpikeInterface/probeinterface, https://github.com/SpikeInterface/spikeinterface, https://github.com/NeuralEnsemble/python-neo

current gpu dev...

```bash
mamba create -n dart python=3.12 pytorch-gpu cupy dask-jobqueue seaborn scikit-learn pytest opt-
einsum h5py "scipy>=1.15" numba pydantic tqdm ipywidgets ipykernel spikeinterface pytest-cov
```

# envs

Get mambaforge: https://github.com/conda-forge/miniforge

The below stuff only works with `mamba`, `conda` has trouble getting env `a` together.

```bash
mamba create -n jupy python=3.11 "jupyterlab>=4.1.0,<5.0.0a0" jupytext ipywidgets widgetsnbextension nodejs nb_conda_kernels black jupyterlab-lsp python-lsp-server ipympl -c conda-forge
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

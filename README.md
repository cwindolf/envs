# envs

```bash
mamba create -n jupy python=3.10 jupyterlab jupytext ipywidgets widgetsnbextension nodejs nb_conda_kernels
mamba activate jupy
jupyter labextension install @ryantam626/jupyterlab_sublime
```

```bash
mamba create -n a numba seaborn scikit-learn scikit-image ipywidgets h5py colorcet tqdm joblib hdbscan cython
mamba activate a
# go to pytorch.org and find install instructions if you want gpu!
mamba install pytorch torchvision torchaudio -c pytorch
pip install matplotlib_venn
pip install -e ~/spikeinterface/ ~/spike-psvae/ ~/dredgefigs/
```

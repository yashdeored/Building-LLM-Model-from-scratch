# Building-LLM-Model-from-scratch

First we need to make directory namely 'fcc-gpt' then we need to install some necessary librarires such as numpy, pylzma, ipykernel and jupyter: 
```
mkdir fcc-gpt
cd fcc-gpt
pip3 install matplotlib numpy pylzma ipykernel jupyter
```
then we need to install torch:
```
pip3 install torch
```

then we need to create a kernel in Jupyter Notebook
if ipykernel is not installed, install it using different command:
```
pip install ipykernel
python -m ipykernel install --user --name=cuda --display-name="cuda-gpt"
```

sometimes there might be problems running in pytorch installation for mac users for that use:

```
conda install pytorch -c pytorch-nightly
```
e

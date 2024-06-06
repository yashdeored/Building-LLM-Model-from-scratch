# Building LLMs from Scratch

## Google Colab for those who don't have a GPU: https://colab.research.google.com/drive/1_7TNpEEl8xjHlr9JzKbK5AuDKXwAkHqj?usp=sharing

Dependencies (assuming windows): `pip install pylzma numpy ipykernel jupyter torch --index-url https://download.pytorch.org/whl/cu118`

If you don't have an NVIDIA GPU, then the `device` parameter will default to `'cpu'` since `device = 'cuda' if torch.cuda.is_available() else 'cpu'`. If device is defaulting to `'cpu'` that is fine, you will just experience slower runtimes.

## All the links you should need are in this repo. I will add detailed explanations as questions and issues are posted.

## Visual Studio 2022 (for lzma compression algo) - https://visualstudio.microsoft.com/downloads/

## OpenWebText Download - https://skylion007.github.io/OpenWebTextCorpus/

How to SSH from Mac to Windows - https://www.youtube.com/watch?v=7hBeAb6WyIg&t=

How to Setup Jupyter Notebooks in 5 minutes or less - https://www.youtube.com/watch?v=eLmweqU5VBA&t=

## Research Papers:
Attention is All You Need - https://arxiv.org/pdf/1706.03762.pdf

A Survey of LLMs - https://arxiv.org/pdf/2303.18223.pdf

QLoRA: Efficient Finetuning of Quantized LLMs - https://arxiv.org/pdf/2305.14314.pdf

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
then we need to create a kernel in Jupyter Notebook if ipykernel is not installed, install it using different command:
```
pip install ipykernel
python -m ipykernel install --user --name=cuda --display-name="cuda-gpt"
```
sometimes there might be problems running in pytorch installation for mac users for that use:
```
conda install pytorch -c pytorch-nightly
```

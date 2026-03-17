# Learn [`einops`](https://einops.rocks/)

- [`einops` tutorials](https://einops.rocks/1-einops-basics/)
- [`einops` paper](https://openreview.net/pdf?id=oapKSVM2bcj)
- Inspired by [Einstein summation notation](https://en.wikipedia.org/wiki/Einstein_notation)
- [Einsum in Deep Learning](https://rockt.ai/2018/04/30/einsum)
- [`einops` git repo](https://github.com/arogozhnikov/einops/)
- [Einops is all you need](https://cxtraa.github.io/machine-learning/einops-arena.html) (Quick reference of key tensor operations with `rearrange`, `reduce` and `einsum`)

I copied some code and resources from the offial repo in order to follow along with the examples in the doc.

# Setup

Install and use [`uv`](https://docs.astral.sh/uv/) to manage the python project, environments and run
scripts within the context of the environment.

This repo is [`uv` project](https://docs.astral.sh/uv/guides/projects) and runs runs scripts
and install dependencies in its isolated python environment.

To update the environment manually, of if you don't see the `.venv` folder in the project root, run

```bash
uv sync
```

You can run the Jupyter notebooks (`.ipynb`) in VS Code using the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter)

Make VS Code Jupyter extension is using the project's environment to execute code. If it prompts to you
choose an environment, select custom path and enter `.venv/bin/python`.

The python environment in use is displayed at the top right corner of the notebook.

![Python env disabled in VS Code notebook](vscode-notebook-python-env.png)

# Notebooks

I use notebooks to experiment with various `einops` functions and concepts as I'm learning:

- [`01-basics.ipynb`](./01-basics.ipynb): The basics, based on [the basics page of the official tutorial](https://einops.rocks/1-einops-basics/)
- [`02-deep-learning.ipynb`](./02-deep-learning.ipynb): Working with deep learning packages, based on [the deep learning section of the official tutorial](https://einops.rocks/2-einops-for-deep-learning/)
- [`03-einsum.ipynb`](./03-einsum.ipynb): Demontrates the `einsum` using various matrix and vector operations. Based on various einsum and einops blog posts: [Einsum is all you need](https://rockt.ai/2018/04/30/einsum), [Einops is all you need](https://cxtraa.github.io/machine-learning/einops-arena.html)

# Basics in data handling

[Nibabel](https://nipy.org/nibabel/) and [Nilearn](https://nilearn.github.io/stable/index.html) are two `python packages` that help to `load`, `modify`, `save` and `visualize neuroimaging data`.
The two software packages together allow you to do almost anything with your `MRI data` that you want. In order to provide a quick introduction and overview of their functionality and capabilities we prepared two short notebooks that will showcase that. 

Additionally, we will have a look at how we can query and extract information from [BIDS](https://bids-specification.readthedocs.io/en/stable/) `datasets` using the [pybids](https://bids-standard.github.io/pybids/index.html) package and outine important aspects of `data management`.

You can find all sections in the `ToC` on the left.

## Nibabel

`Nibabel`'s main focus is on `loading` and `saving` any kind of `neuroimaging data`.

<img src="https://nipy.org/nibabel/_static/nibabel-logo.svg" alt="workshop logo" width="200" style="margin:0 0 0 0"/>

## Nilearn

`Nilearn`'s main focus is on `statistical learning` (based on [scikit-learn]()) but is also very good in `manipulation` and `visualizing neuroimaging data`.

<img src="https://nilearn.github.io/stable/_static/nilearn-transparent.png" alt="workshop logo" width="200" style="margin:0 0 0 0"/>

## Pybids, standardization & data management

`Pybids` is a `python package` that allows you to `query` and `extract` information from `BIDS datasets`. The tutorial showcases its functionality based on a couple of example datasets. Speaking of `BIDS`, to provide a more hollistic view while also introducing important concepts and providing a rationale, we will talk about `data management` and `data organization` in the context of `neuroimaging`. You can find this content in the `slide deck` below.

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTx_4omqcaJv2VqBSz2lKAdReSJkyFnm1o-I2dL62DU--_yBRh8bkTXtfzOuuwjNvlYw0sC2zDjzQ_N/embed?start=false&loop=false&delayms=3000" frameborder="0" width="700" height="430" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
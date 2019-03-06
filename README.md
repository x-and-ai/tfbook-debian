# xandai/tfbook-debian

[Docker Hub Link](https://hub.docker.com/r/xandai/tfbook-debian)

[GitHub Link](https://github.com/x-and-ai/tfbook-debian)

## Description

This is a Docker image for using TensorFlow with Python 3 and Jupyter on Debian.

This image also contains following packages:

NumPy (for low-level math operations)
pandas (for data manipulation)
scikit-learn (for evaluation metrics)
imageio (for read and write images)
Matplotlib (for data visualization)
Seaborn (for heatmaps)

## Tags and Versions

| tag        | tensorflow | numpy      | pandas     | scikit-learn | imageio    | matplotlib | seaborn    | jupyter    | python     | debian     |
|:----------:|:----------:|:----------:|:----------:|:------------:|:----------:|:----------:|:----------:|:----------:|:----------:|:----------:|
| 1.0.0      | 1.13.1     | 1.16.2     | 0.24.1     | 0.20.3       | 2.5.0      | 3.0.3      | 0.9.0      | 1.0.0      | 3.5.3-1    | 9.8        |

## Usage

- Start notebook without token

``` sh
docker run --rm -it -p <localhostport>:8888 -v /absolute/path/to/notebook/dir:/home/jupyter/notebook xandai/tfbook-debian:1.0.0 jupyter notebook --NotebookApp.token=''
```

- Start notebook with token

``` sh
docker run --rm -it -p <localhostport>:8888 -v /absolute/path/to/notebook/dir:/home/jupyter/notebook xandai/tfbook-debian:1.0.0
```

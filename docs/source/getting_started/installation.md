% Copyright (c) Jupyter Development Team.

% Distributed under the terms of the Modified BSD License.

(installation)=

# Installation

JupyterLab can be installed as a terminal-launched application accessible via a web browser (default), or as a desktop application which 
of JupyterLab and any related tools that are critical to your workflows.
:::

## conda

If you use `conda`, you can install it with:

```bash
conda install -c conda-forge jupyterlab
```

## mamba

If you use `mamba`, you can install it with:

```bash
mamba install -c conda-forge jupyterlab
```

## uv

If you use `uv`, you can install it with:

```bash
uv tool install jupyterlab --with pip
```

## 
Alternatively, you can run `jupyter lab` inside the virtualenv with

```bash
pipenv run jupyter lab
```

## Docker

If you have [Docker installed](https://docs.docker.com/install/), you can install and use JupyterLab by selecting one
of the many [ready-to-run Docker images](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html)
maintained by the Jupyter Team. Follow the instructions in the [Quick Start Guide](https://jupyter-docker-stacks.readthedocs.io/en/latest/)
to deploy the chosen Docker image.

Ensure 

## Supported browsers

The latest versions of the following browsers are currently known to work:

- Firefox
- Chrome
- Safari
- Edge

Earlier browser versions may also work, but come with no guarantees.

## Installation problems

If your computer is behind corporate proxy or firewall,
you may encounter HTTP and SSL errors due to the proxy or firewall blocking connections to widely-used servers. For example, you might see this error if conda cannot connect to its own repositories:

```
CondaHTTPError: HTTP 000 CONNECTION FAILED for url <https://repo.anaconda.com/pkgs/main/win-64/current_repodata.json>
```

Here are some widely-used sites that host packages in the Python and JavaScript open-source ecosystems. Your network administrator may be able to allow http and https connections to HTTP_PROXY=http://USER:PWD@proxy.company.com:PORT
export HTTPS_PROXY=https://USER:PWD@proxy.company.com:PORT
```

In case you can communicate via HTTP, but installation with `conda` dependencies. If `npm` cannot connect to its own repositories, you might see an error like:

```
ValueError: "@jupyterlab/toc" is not a valid npm package
```

You can set the proxy or registry used for npm with the following commands.

```bash
# Set proxy for NPM
npm config set proxy http://USER:PWD@proxy.company.com:PORT
npm config set proxy https://USER:PWD@proxy.company.com:PORT

# Set default registry for NPM (optional, useful in case if common JavaScript libs cannot be found)
npm 

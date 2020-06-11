# EC-Argovis-API-Demo
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/tylertucker202/EC-Argovis-API-Demo/master?urlpath=https%3A%2F%2Fgithub.com%2Ftylertucker202%2FEC-Argovis-API-Demo%2Fblob%2Fmaster%2FEC2020_argovis_python_api.ipynb)
## Demonstration of Argovis Python API - For Earthcube 2020 meeting

You can run these notebooks using your own Jupyter kernel. 

The notebooks use some libraries that can take time to set up on some systems (e.g. Cartopy).

I've created a Dockerfile to make this install easier. 

This project assumes that [Docker](https://www.docker.com/) is installed on your PC, and that the daemon is running. Additionally, make sure that port 8888 is open. Check with `lsof -i :8888`.

First, open a terminal

Then build the image with the following command

`docker build --no-cache -t argovis_python_api_demo:1.0 .`

Run the image with this code in a Linux terminal or Windows PowerShell

`docker run  -v ${PWD}:/usr/src/av_py_env -p 8888:8888 argovis_python_api_demo:1.0`

Lastly, follow the provided link in the terminal. You may be prompted to set the kernel on a notebook. Just set the kernel to av_py_env. Good luck!

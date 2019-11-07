# Dask Trial Container - Set up instructions.
1. docker run --name dask_trial -p 8888:8888 -p 8787:8787 -e GRANT_SUDO=yes --user root -v D:\local-sectra\03_developments\data-science\dask_tutorial:/home/jovyan/work jupyter/base-notebook:latest
2. docker exec -it dask_trial bash
3. conda install dask
4. apt-get update
5. apt-get install graphviz
6. conda install python-graphviz

To start the container:
1. docker start dask_trial -a
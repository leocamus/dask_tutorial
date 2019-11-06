# Dask Trial Container - Set up instructions.
1. docker run --name dask_trial -p 8888:8888 -p 8787:8787 -e GRANT_SUDO=yes --user root -v D:\local-sectra\03_developments\data-science\dask_trial:/home/jovyan/work jupyter/base-notebook:latest
2. docker exec -it dask_trial bash
3. cd work
4. pip install -r requirements.txt
5. apt-get update
6. apt-get install graphviz
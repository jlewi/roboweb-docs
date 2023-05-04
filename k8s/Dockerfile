# Use Kubeflow image as base image
# This appears to be a bit outdated but lets try it
FROM public.ecr.aws/j1r0q0g6/notebooks/notebook-servers/jupyter:v1.5.0

USER root
# Kubeflow ships jupyter-server 1.13 which is out of date. The server is on 2.5
RUN python3 -m pip uninstall -y jupyter jupyter-server
RUN python3 -m pip install --upgrade jupyter jupyter-server==2.5.0 jupyterlab
RUN python3 -m pip install roboweb-extension roboweb-server
RUN python3 -m jupyter serverextension enable --py roboweb_server
USER jovyan

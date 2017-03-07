# jupyter-opencv

Jupyter notebook with OpenCV bindings added.

## Build

docker build -t kscape/jupyter-opencv .

## Run

This command runs it so you can connect at localhost using ssl with no token required.

docker run --name jupyter -d -p 443:8888 -v $(pwd)\notebooks:/home/jovyan/work kscape/jupyter-opencv start-notebook.sh --NotebookApp.token=''
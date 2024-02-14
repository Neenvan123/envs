FROM intel4coro/base-notebook:20.04-noetic-full-xpra

WORKDIR /app

COPY . /app/

RUN pip uninstall -y jlab-enhanced-cell-toolbar
RUN pip install https://raw.githubusercontent.com/yxzhan/jupyterlab-rviz/master/dist/jupyterlab_rviz-0.3.2.tar.gz \
  https://raw.githubusercontent.com/yxzhan/extension-examples/main/cell-toolbar/dist/jupyterlab_examples_cell_toolbar-0.1.4.tar.gz
RUN mamba install -y ripgrep
RUN pip install --upgrade \
  sidecar \
  Cython \
  jupyterlab-git \
  jupyterlab-unfold \
  jupyter-archive \
  jupyterlab-search-replace \
  jupyter-offlinenotebook \
  jupyterlab-language-pack-de-DE  \
  jupyterlab_execute_time


RUN pip install --upgrade \
  jupyter-collaboration \
  openai \
  jupyter-ai \
  rasa \
  spacy
ARG TAG
ARG JUPYTERLAB_VERSION

FROM ydata/jupyterlab-${JUPYTERLAB_VERSION}:${TAG}

COPY --chown=ydata:users requirements.txt /tmp/

RUN pip --no-cache-dir install -r /tmp/requirements.txt

RUN pip uninstall pip -y
FROM cargo.caicloud.xyz/devops_release/miniconda:v4.7.12.1-py36

# Install mxnet
ARG MXNET_VERSION=1.5.0
ARG MXNET_TYPE=mxnet
RUN pip install --no-cache-dir ${MXNET_TYPE}==${MXNET_VERSION} onnx

## Install horovod with mxnet
ARG HOROVOD_VERSION=0.19.0
RUN HOROVOD_WITH_MXNET=1 pip install --no-cache-dir horovod==${HOROVOD_VERSION}

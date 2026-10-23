ARG RENDERCV_VERSION=2.8

FROM python:3.12-slim
ARG RENDERCV_VERSION

RUN apt-get update && apt-get upgrade -y

RUN pip install --force-reinstall -v "rendercv[full]==${RENDERCV_VERSION}"

WORKDIR /cv

ENTRYPOINT [ "rendercv" ]

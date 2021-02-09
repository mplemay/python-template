FROM mcr.microsoft.com/vscode/devcontainers/python:3.9

RUN apt update && \
	DEBIAN_FRONTEND=noninteractive apt upgrade -y && \
	DEBIAN_FRONTEND=noninteractive apt install -y fish

COPY requirements.txt /tmp/pip-tmp/
RUN pip3 --disable-pip-version-check --no-cache-dir install -r /tmp/pip-tmp/requirements.txt && \
    rm -rf /tmp/pip-tmp

FROM mcr.microsoft.com/vscode/devcontainers/python:3.8

ADD requirements.txt /tmp/.
RUN python3 -m pip insall pip setuptools --no-cache-dir --upgrade && \
	python3 -m pip install -r /tmp/requirements.txt --no-cache-dir --upgrade

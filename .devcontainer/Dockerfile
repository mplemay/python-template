FROM mcr.microsoft.com/vscode/devcontainers/python:3.9

RUN apt update && \
	DEBIAN_FRONTEND=noninteractive apt upgrade -y && \
	DEBIAN_FRONTEND=noninteractive apt install -y fish

ARG POETRY_HOME=/opt/poetry
RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python3 && \
	chmod a+x /opt/poetry/bin/poetry
ENV PATH="/opt/poetry/bin:$PATH"

FROM opencadc/astropy-5:3.10-slim

RUN apt-get update \
    && apt-get install -y \
        build-essential \
        gcc \
        gfortran \
        libblas-dev \
        libc-dev \
        libffi-dev \
        libfreetype6-dev \
        libmagic-dev \
        libpng-dev \
        libssl-dev \
        libxslt-dev \
        make

RUN pip --no-cache-dir install matplotlib

RUN apt-get clean \
    && apt-get autoclean \
    && rm -rf /var/lib/apt/lists/*

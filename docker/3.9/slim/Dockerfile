FROM opencadc/astropy:3.9-slim

RUN apt update \
    && apt install -y \
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

RUN apt clean \
    && apt autoclean \
    && rm -rf /var/lib/apt/lists/*

Bootstrap:docker
From:ubuntu:latest

%labels
Maintainer: Zac Stephens

%environment

$post
  # Most from chpc ubuntu build def
  mkdir /uufs
  mkdir /scratch
  apt-get && update apt-get install -y --no-install-recommends \
  apt-utils \
  build-essential \
  curl \
  git \
  libopenblas-dev \
  libcurl4-openssl-dev \
  libfreetype6-dev \
  libpng-dev \
  libzmq3-dev \
  mpich \
  python-pip \
  pkg-config \
  python-dev \
  python-setuptools \
  rsync \
  software-properties-common \
  unzip \
  vim \
  wget \
  zip \
  zlib1g-dev
  apt-get clean

  #MC issue with locale (LC_ALL, LANGUAGE), to get it right:
  apt-get install -y language-pack-en
  locale-gen "en_US.UTF-8"
  dpkg-reconfigure locales
  export LANGUAGE="en_US.UTF-8"
  echo 'LANGUAGE="en_US.UTF-8"' >> /etc/default/locale
  echo 'LC_ALL="en_US.UTF-8"' >> /etc/default/locale

%runscript

%test

%environment

%files

%help

Bootstrap:docker
From:nfcore/base

%post

    /opt/conda/bin/conda env create -f /environment.yml
    /opt/conda/bin/conda clean -a
    mkdir -p /ifs
    apt-get -y install procps unzip
    mkdir -p /opt/trimmomatic && cd /opt/trimmomatic && wget http://www.usadellab.org/cms/uploads/supplementary/Trimmomatic/Trimmomatic-0.36.zip \
        && unzip Trimmomatic-0.36.zip && mv Trimmomatic-0.36 0.36 && rm Trimmomatic-0.36.zip

    cd /opt

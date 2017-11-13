BootStrap: docker
From: ubuntu:16.04

%post
    apt-get -y update
    apt-get -y install wget npm nodejs-legacy vim git
    wget https://repo.continuum.io/archive/Anaconda3-5.0.1-Linux-x86_64.sh
    bash Anaconda3-5.0.1-Linux-x86_64.sh -b -p /opt/anaconda
    rm Anaconda3-5.0.1-Linux-x86_64.sh
    export PATH=/opt/anaconda/bin:$PATH
    conda install -y -c conda-forge jupyterhub
    conda install -y notebook
    mkdir /hgcb
    
%environment
    export PATH=/opt/anaconda/bin:$PATH

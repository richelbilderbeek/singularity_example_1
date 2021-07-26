BootStrap: debootstrap
OSVersion: trusty
MirrorURL: http://us.archive.ubuntu.com/ubuntu/

%runscript
    echo "My root folder: "
    ls /
    echo "My operating system: "
    cat /etc/*-release

%post
    echo "Hello from inside the container"
    sed -i 's/$/ universe/' /etc/apt/sources.list
    apt-get update
    apt-get -y install vim
    apt-get clean

%labels

    AUTHOR Richel J.C. Bilderbeek

    NAME singularity_example_1
 
    DESCRIPTION Singularity example 1: Singularity and Ubuntu

    USAGE simply run the container

    URL https://github.com/richelbilderbeek/singularity_example_1

    VERSION 1.0

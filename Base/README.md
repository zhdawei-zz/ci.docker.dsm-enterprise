#Building an IBM Data Server Manager Base image from binaries
 
An IBM Data Server Manager Base image can be built by obtaining the following binaries:

IBM Data Server Manager from [developerworks](http://www.ibm.com/developerworks/downloads/im/dsm/)


IBM Data Server Manager image is created by using the following Dockerfiles:

    Dockerfile

Dockerfile:

    Uses the image created by Dockerfile as the base image

    Copies the server startup script to the image

    When the container is started the server is started

Building the IBM Data Server Manager Base image

    Place the downloaded IBM Data Server Manager binaries and unpack to ibm-datasrvrmgr

    Edit setup.conf

    Place start_dsm.sh

    Download the ubuntu 14.04 image

    docker pull ubuntu:14.04

    Move to the directory base/

    Build the prereq image by using:

docker build  -t <prereq-image-name> -f Dockerfile.install .
                            
Running the images

Using the IBM Data Server Manager Base traditional install image 

FROM biocontainers/biocontainers:debian-stretch-backports
MAINTAINER biocontainers <biodocker@gmail.com>
LABEL    software="autogrid-test" \ 
    container="autogrid-test" \ 
    about.summary="test files for AutoGrid" \ 
    about.home="http://autodock.scripps.edu/" \ 
    software.version="4.2.6-3-deb" \ 
    version="1" \ 
    about.copyright="1989-2014, All Rights Reserved." \ 
    about.license="GPL-2+" \ 
    about.license_file="/usr/share/doc/autogrid-test/copyright" \ 
    about.tags="field::biology, field::biology:structural, made-of::TODO, role::TODO,:app-data, use::TODO, use::checking" 

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install -y autogrid-test && apt-get clean && apt-get purge && rm -rf /var/lib/apt/lists/* /tmp/*
USER biodocker

# Dockerfile for bamboofox github pages
FROM jekyll/jekyll:latest
MAINTAINER bruce30262

# locale
ENV LANG en_US.UTF-8  
ENV LANGUAGE en_US:en  
ENV LC_ALL en_US.UTF-8

# clone repo & install 
RUN git clone https://github.com/bruce30262/bamboofox.github.io.git ~/bamboofox.github.io
RUN cd ~/bamboofox.github.io && bundle install

# cmd
WORKDIR ~/bamboofox.github.io
CMD ["/bin/bash"]

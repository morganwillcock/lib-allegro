FROM debian:jessie

# Take default debconf options
ENV DEBIAN_FRONTEND noninteractive

# Always say yes to apt-get operations
RUN echo 'APT::Get::Assume-Yes "true";' >> /etc/apt/apt.conf

# Upgrade existing packages
RUN apt-get update && apt-get upgrade

# Get build dependencies
RUN apt-get install \
  build-essential \
  cmake \
  git \
  libasound2-dev \
  libjack-dev \
  libsdl2-dev \

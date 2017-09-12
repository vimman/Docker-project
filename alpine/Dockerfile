FROM alpine:latest

MAINTAINER Vimman

RUN apk update

RUN apk add zsh \
			neovim \
			git \
			curl

RUN git clone https://github.com/vimman/dotfiles.git/ /home/dotfiles

WORKDIR /home

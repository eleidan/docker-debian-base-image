FROM debian:jessie
MAINTAINER Oleg Kulyk

RUN touch /etc/skel/.bash_history

ENV HOME="/root" \
    SERVICE_NAME="debian:jessie" \
    CONTAINER_PS1="[ $(get_container_ip) | \[\e[0;36m\]$(get_container_service)\[\e[m\] | \[\e[0;35m\]\w\[\e[m\] ]\n\[\e[1;31m\]>\[\e[m\] "

COPY .bashrc .bash_customizations $HOME/

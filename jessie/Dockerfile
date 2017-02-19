FROM debian:jessie
MAINTAINER Oleg Kulyk

COPY .profile .bashrc .bash_history .bash_customizations  /etc/skel/

ENV HOME="/root" \
    SERVICE_NAME="debian:jessie" \
    CONTAINER_PS1="[ $(get_container_ip) | \[\e[0;36m\]$(get_container_service)\[\e[m\] | \[\e[0;35m\]\w\[\e[m\] ]\n\[\e[1;32m\]>\[\e[m\] "

COPY .profile .bashrc .bash_history .bash_customizations  $HOME/

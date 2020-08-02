FROM archlinux/base

WORKDIR /home/ocamlproj

RUN pacman -Syu --noconfirm && pacman -S --noconfirm ocaml && \
	pacman -Sy --noconfirm vim && pacman -Sy --noconfirm git
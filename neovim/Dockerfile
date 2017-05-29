FROM alpine

RUN apk --update add curl tmux neovim-doc neovim

RUN curl -fLo /home/.config/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

ADD https://raw.githubusercontent.com/vimman/dotfiles/master/nvim/init.vim \
	/home/.config/nvim/init.vim

WORKDIR	/tmp

ENTRYPOINT tmux -c nvim

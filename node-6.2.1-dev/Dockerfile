FROM node:6.2.1

RUN git config --global alias.st status \
 && git config --global alias.co checkout \
 && git config --global alias.ci commit \
 && git config --global alias.br branch

##################
# Install software
##################

RUN apt-get update \

&& apt-get install -y vim \

# Oh My Zsh
&& apt-get install -y zsh \
&& git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh \
&& cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc \
&& chsh -s /bin/zsh

##################

WORKDIR /usr/src/app

EXPOSE 3000

CMD [ "/bin/zsh" ]

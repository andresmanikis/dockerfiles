FROM node:6.2.1

RUN git config --global alias.st status \
 && git config --global alias.co checkout \
 && git config --global alias.ci commit \
 && git config --global alias.br branch

WORKDIR /usr/src/app

EXPOSE 3000

CMD [ "/bin/bash" ]

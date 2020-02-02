# build using "docker build . -t heroku"
FROM ubuntu

LABEL Name=heroku Version=0.0.2

WORKDIR /app



RUN apt update
RUN apt install nano git curl -y
RUN git config --global user.email "me@localhost"
RUN git config --global user.name "me"
RUN curl https://cli-assets.heroku.com/install.sh | sh
RUN touch Procfile

#copy files
ADD . /app

#login using heroku login
CMD ["bash" ]

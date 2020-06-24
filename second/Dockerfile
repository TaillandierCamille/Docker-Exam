# BASE
FROM debian

# INSTALL
RUN apt-get update -y \
    && apt-get install -y git  \
    && apt-get install -y curl

RUN curl -sL "https://deb.nodesource.com/setup_12.x" | bash - \
    && apt-get install -y nodejs


# expose
EXPOSE 3000/tcp

# COMMANDS
RUN git clone "https://github.com/jponcy/fake-game-api.git" 

CMD npm install \
    && bash npm run start:separed
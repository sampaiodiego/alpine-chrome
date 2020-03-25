FROM chinello/alpine-chrome

USER root
RUN apk add --no-cache tini@edge make@edge gcc@edge g++@edge python@edge git@edge nodejs@edge nodejs-npm@edge yarn@edge \
	&& rm -rf /var/lib/apt/lists/* \
    /var/cache/apk/* \
    /usr/share/man \
    /tmp/*
USER chrome
ENTRYPOINT ["tini", "--"]

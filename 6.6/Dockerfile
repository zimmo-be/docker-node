FROM node:6.6

RUN mkdir -p /usr/src/app \
    && useradd --user-group --home-dir /usr/src/app --shell /bin/false app \
    && chown -R app:app /usr/src/app \
    && npm install -g nodemon babel-cli pm2

USER app

WORKDIR /usr/src/app

EXPOSE 3000

CMD [ "npm", "start" ]

FROM node:14

ARG DIR=/app

ENV SERVICE=http://localhost:3000
# user
RUN useradd -m thaint

USER thaint

WORKDIR $DIR

COPY package.json .

RUN npm install

COPY ./app.js .

EXPOSE 3000

CMD ["node", "app.js"]


# ADD https://github.com/soumyajit4419/Portfolio.git .

# CMD ["echo", "Hello world"]
# ENTRYPOINT ["echo", "Hello world"]
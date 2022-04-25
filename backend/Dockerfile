FROM node: 12.alphine

RUN mkdir -p /app

WORKDIR /app

COPY packaje*.json /app/

RUN npm i

COPY . /app/

CMD:  [*npm*.*start*]

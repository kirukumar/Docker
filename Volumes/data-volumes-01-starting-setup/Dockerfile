FROM node:14

WORKDIR /app/

COPY package.json .

RUN npm install

#COPY . . (This line is also not needed for bindmounts as we are using only )
#ENV PORT=3000

ARG DEFAULT_PORT

ENV PORT=$DEFAULT_PORT

EXPOSE $PORT

CMD [ "npm","start" ]
FROM node:16.0

WORKDIR /usr/src/app

EXPOSE 5000


COPY package* ./

RUN npm install

COPY . . 

ENV REACT_APP_BACKEND_URL=http://localhost:8080
RUN REACT_APP_BACKEND_URL=http://localhost:8080 npm run build

RUN npm install -g serve

CMD ["serve", "-s", "-l", "5000", "build"]


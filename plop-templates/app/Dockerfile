FROM node:8.2


#RUN apt-get update
#RUN apt-get install git -y

RUN git clone https://github.com/vyom00/prefab-ui-universal.git

RUN yarn install -w -y

WORKDIR "/prefab-ui-universal/packages/app"

#RUN docker build -t next-app .


RUN  npm install

RUN npm run-script build
RUN npm start
RUN npm run generate --component react-app

FROM node:12-stretch

RUN echo "Europe/Amsterdam" > /etc/timezone
RUN dpkg-reconfigure -f noninteractive tzdata

COPY . /app
RUN npm install
WORKDIR /app


CMD ["npm", "start"]

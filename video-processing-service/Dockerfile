# Use an offical Node runtime as a parent image
FROM node:18

# Set teh working director in the container to /app
WORKDIR /app

COPY package* .json ./

RUN apt-get update && apt-get install -y ffmpeg

Run npm install

COPY . .

EXPOSE 3000

CMD ["npm","start"]

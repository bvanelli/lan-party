FROM node:21
WORKDIR /app
RUN apt-get update && apt-get install -y git
RUN git clone https://github.com/huytd/agar.io-clone.git
RUN cd agar.io-clone && npm install

WORKDIR /app/agar.io-clone
ENTRYPOINT ["npm", "run", "start"]

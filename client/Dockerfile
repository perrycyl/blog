FROM node:alpine

ENV CI=true

# # Copy npm config
# COPY .npmrc /root/.npmrc

WORKDIR /app
COPY package.json ./
#Connection issue causing error. Forcing unsafe npm installation with extending timeout to bypass.
RUN npm install --loglevel verbose -timeout=9999999 -registry=http://registry.npmjs.org/
COPY ./ ./

CMD [ "npm","start" ]

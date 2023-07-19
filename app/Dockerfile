FROM node:18-slim

USER node

WORKDIR /home/node
COPY --chown=node:node package*.json ./

RUN npm install --only=production
COPY . .

# Run service.
CMD [ "npm", "start" ]

#only node and npm included in this alpine image nothing much
FROM node:14-alpine
COPY ./ ./
RUN npm install
CMD ["npm", "start"]
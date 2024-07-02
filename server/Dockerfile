FROM node:16.17.0-alpine
WORKDIR /app
COPY ./package.json .
COPY ./package-lock.json .
RUN npm install
COPY . .
#ENV MONGO_URI=mongodb://${MONGO_SRV}/
ENV MONGO_URI=mongodb://mongoserver/

#RUN yarn build
EXPOSE 5000
CMD ["npm", "start"]

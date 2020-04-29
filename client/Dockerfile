#Build Phase

FROM node:alpine as builder

WORKDIR '/app'

COPY package*.json ./

RUN npm install

COPY . . 
#no need for volumes here bcz in production environment we
#do not need to change the code at all. So copy whole code to the container.

RUN npm run build 


#Run Phase

FROM nginx
EXPOSE 3000

COPY ./nginx/default.conf /etc/nginx/conf.d/default.conf

COPY --from=builder /app/build /usr/share/nginx/html

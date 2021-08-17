FROM nginx:latest

RUN apt-get update && apt-get install -y procps curl

COPY default.conf /etc/nginx/conf.d/default.conf

ADD search.html  /usr/share/nginx/html

ADD css /usr/share/nginx/html/css

ADD fonts /usr/share/nginx/html/fonts

#ADD data /usr/share/nginx/html/data 

EXPOSE 1234

CMD ["nginx", "-g", "daemon off;"]

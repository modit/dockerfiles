FROM node:0.10

EXPOSE 80

RUN apt-get update -qq && apt-get install -qqy \
	build-essential \
	gcc \
	make \
	python \
	> /dev/null

RUN npm install -g \
	grunt-cli \
	nan \
	node-gyp

WORKDIR /usr/src/app
CMD node
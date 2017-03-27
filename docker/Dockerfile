FROM ruby:2.4.1-alpine
ENV packages ruby-dev build-base

RUN apk update && \
	apk upgrade && \
	apk add $packages && \
	gem install rails && \
	apk del $packages
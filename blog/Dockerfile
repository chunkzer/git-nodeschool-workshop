FROM ruby:2.2-slim
RUN apt-get update -qq && apt-get install -y build-essential libmysqlclient-dev
RUN mkdir /blog
WORKDIR /blog
ADD Gemfile /blog/Gemfile
RUN bundle install
ADD . /blog

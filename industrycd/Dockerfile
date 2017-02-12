FROM ruby:2.3.1
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
 
 
RUN mkdir /indsutrycd
WORKDIR /tmp
COPY Gemfile Gemfile
COPY Gemfile.lock Gemfile.lock
RUN bundle install -j 4
 
ADD . /indsutrycd
WORKDIR /indsutrycd

FROM ruby:3.0.0
RUN apt-get update -qq && apt-get install -y nodejs postgresql-client
WORKDIR /aplicacao
COPY Gemfile /aplicacao/Gemfile
COPY Gemfile.lock /aplicacao/Gemfile.lock
RUN bundle install
CMD ["rails", "server", "-b", "0.0.0.0"]

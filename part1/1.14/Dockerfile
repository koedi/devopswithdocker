FROM ruby:2.6.0

WORKDIR /mydir

RUN apt update && apt install -y git
RUN git clone https://github.com/docker-hy/rails-example-project /mydir

RUN apt install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x
RUN apt install -y nodejs

RUN gem install bundler
RUN bundle install
RUN rails db:migrate

EXPOSE 3000

CMD ["rails","s"]

FROM ruby:2.6.3

WORKDIR /usr/src/test

RUN gem install watir \
    && apt-get update \
    && apt-get install jq -y

COPY wait-for-grid.sh bulletin_board.rb /usr/src/test/

RUN chmod +x wait-for-grid.sh

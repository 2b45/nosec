FROM ruby:2.3

MAINTAINER <xx-zhang actanble@gmail.com>

ENV WHATWEB_VERSION master
RUN git clone --branch $WHATWEB_VERSION https://github.com/urbanadventurer/WhatWeb.git /src/whatweb

#RUN  gem sources -a http://gems.ruby-china.com/
#RUN gem sources --add https://ruby.taobao.org/

# https://github.com/urbanadventurer/WhatWeb/wiki/Installation
RUN gem install rchardet mongo json
RUN cd /src/whatweb && bundle install

WORKDIR /src/whatweb

CMD /src/whatweb/whatweb
FROM ruby:latest
LABEL maintainer="taichunmin@gmail.com"
ENV LANG=C.UTF-8 LC_ALL=C.UTF-8 LANGUAGE=C.UTF-8 DEBIAN_FRONTEND=noninteractive

WORKDIR /root

RUN \
    gem install asciidoctor rouge pygments.rb coderay && \
    gem install asciidoctor-pdf --pre && \
    gem install asciidoctor-pdf-cjk-kai_gen_gothic && \
    NOKOGIRI_USE_SYSTEM_LIBRARIES=1 gem install asciidoctor-epub3 --pre && \
    asciidoctor-pdf-cjk-kai_gen_gothic-install
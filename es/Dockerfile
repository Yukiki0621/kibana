FROM docker.elastic.co/elasticsearch/elasticsearch:6.3.2

# x-pack をインストール
#RUN elasticsearch-plugin  install --batch x-pack
#RUN elasticsearch-plugin  install analysis-kuromoji

WORKDIR /usr/share/elasticsearch

COPY config ./config
RUN chown -R elasticsearch:elasticsearch /usr/share/elasticsearch/config
USER elasticsearch

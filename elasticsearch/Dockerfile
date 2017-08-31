FROM elasticsearch:5.1.1

COPY elasticsearch.yml config/

RUN mkdir -p /mnt/shared/elasticsearch \
    && chown -R elasticsearch:elasticsearch /mnt/shared/elasticsearch

VOLUME /mnt/shared
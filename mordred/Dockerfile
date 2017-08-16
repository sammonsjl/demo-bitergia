# Copyright (C) 2016 Bitergia
# GPLv3 License

FROM bitergia/mordred:latest

USER root

ADD stage ${DEPLOY_USER_DIR}/stage
COPY conf/ ${DEPLOY_USER_DIR}/conf

RUN mkdir -p /home/bitergia/.perceval \
        && chmod 755 ${DEPLOY_USER_DIR}/stage \
        && chown -R bitergia:bitergia /home/bitergia

VOLUME /home/bitergia/.perceval

USER ${DEPLOY_USER}

CMD ${DEPLOY_USER_DIR}/stage
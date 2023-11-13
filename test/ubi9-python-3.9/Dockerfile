ARG BASE_IMAGE
FROM ${BASE_IMAGE}

LABEL name="TEST"

WORKDIR /opt/app-root/bin

ARG USERNAME
ARG PASSWORD

RUN echo $USERNAME $PASSWORD


RUN chmod -R g+w /opt/app-root/lib/python3.9/site-packages && \
      fix-permissions /opt/app-root -P

WORKDIR /opt/app-root/src


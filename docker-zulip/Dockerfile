FROM zulip/docker-zulip:7.0-0

ARG RENDER_EXTERNAL_HOSTNAME
ENV SETTING_EXTERNAL_HOST=${SETTING_EXTERNAL_HOST:-$RENDER_EXTERNAL_HOSTNAME}
RUN apt-get update && apt-get install -y nano python-dev
RUN chown zulip:zulip /usr/bin/supervisorctl


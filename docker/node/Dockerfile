FROM node:16

# (optional) quiet some npm noise
ENV NPM_CONFIG_FUND=false NPM_CONFIG_AUDIT=false

# Set PROJECT USER
RUN groupmod -g 999 node && usermod -u 999 -g 999 node
RUN useradd -ms /bin/bash project
USER project
WORKDIR /project

CMD tail -f /dev/null

FROM meteorhacks/meteord:base
MAINTAINER mike@mikangali.com

# Install ps cmd required for mongo and tools
RUN apt-get update && apt-get install -y imagemagick procps

# Install meteor
RUN bash $METEORD_DIR/lib/install_meteor.sh

WORKDIR /app

EXPOSE 3000

ENV LANG=C
ENV LC_ALL=C

ENTRYPOINT /bin/bash

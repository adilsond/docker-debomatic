FROM debian:sid
LABEL maintainer=adilson@adilson.net.br
RUN apt-get update -y && apt-get upgrade -y \
    && apt-get install --no-install-recommends ca-certificates nano debomatic -y \ 
    && apt-get clean \
    && rm -rf /etc/debomatic/distributions \
    && wget -O /etc/debomatic/distributions -cq https://raw.githubusercontent.com/debomatic/debomatic/master/etc/debomatic/distributions

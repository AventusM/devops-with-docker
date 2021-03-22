FROM ubuntu:18.04
# Prerequisites
RUN apt-get update && apt-get install -y curl && apt-get clean

COPY fetch.sh .
RUN chmod +x fetch.sh
CMD ./fetch.sh
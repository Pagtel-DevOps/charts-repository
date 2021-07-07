FROM ubuntu:21.10
LABEL maintainer="Santos <lucas.santos@pagtel.com.br>"

RUN apt-get update -yq
RUN apt-get install curl gnupg2 -yq

RUN curl https://baltocdn.com/helm/signing.asc | apt-key add -
RUN apt-get install apt-transport-https -yq
RUN echo "deb https://baltocdn.com/helm/stable/debian/ all main" | tee /etc/apt/sources.list.d/helm-stable-debian.list
RUN apt-get update -yq
RUN apt-get install helm -yq
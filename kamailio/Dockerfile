FROM hashicorp/consul-template:alpine as template

FROM kamailio/kamailio:5.3.1-buster

RUN apt-get -yqq update && apt-get -yqq install procps

COPY --from=template /bin/consul-template /usr/bin/consul-template

ADD ./config/kamailio/* /etc/kamailio/
ADD ./config/consul-template/* /config/

CMD consul-template -log-level debug -config /config/template.hcl
ENTRYPOINT consul-template -log-level debug -config /config/template.hcl
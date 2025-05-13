FROM envoyproxy/envoy:v1.30.0

LABEL maintainer="howudoindante"

WORKDIR /etc/envoy

COPY envoy.yaml ./envoy.yaml

EXPOSE 8080

CMD ["envoy", "-c", "/etc/envoy/envoy.yaml", "--service-node", "gateway", "--service-cluster", "gateway", "--log-level", "debug"]

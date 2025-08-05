# demo_promtheus

# Setup /etc/host
127.0.0.1       host.docker.internal

# Setup Grafana
Prometheus server URL - http://host.docker.internal:30090

# Verify Internal Network
kubectl run -it --rm debug --image=curlimages/curl --restart=Never -- curl -v http://my-demo:9000/actuator/prometheus
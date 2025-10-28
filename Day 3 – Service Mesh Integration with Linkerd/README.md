Day 3 – Service Mesh Integration with Linkerd

# Tasks Completed
  - Installed Linkerd CLI and validated the cluster environment using linkerd check --pre to ensure compatibility.
  - Deployed the Linkerd control plane (identity, destination, proxy injector) into the cluster, which manages communication and security between microservices.
  - Verified successful installation with kubectl get pods -n linkerd, confirming all control-plane components were running.
  - Installed the Linkerd Viz extension, providing built-in observability dashboards for latency, success rates, and request volume.
  - Enabled automatic sidecar injection in the sock-shop namespace
  - Accessed the Linkerd Viz Dashboard to monitor real-time service-to-service communication, golden metrics, and request success rates.
  - Verified all Sock Shop microservices were meshed and communicating securely through Linkerd.

# Screenshots
  - linkerd check output showing successful installation and validation.
  - kubectl get pods -n linkerd → all Linkerd components running.
  - Sock Shop namespace annotated for sidecar injection.
  - Linkerd Viz dashboard showing healthy meshed microservices.

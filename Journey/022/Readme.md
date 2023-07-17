# Probes in K8s

## Cloud Research

- ✍️ I learned about probes in Kubernetes. Probes are used to check the health of a container. There are three types of probes:
    
  - Liveness probe: used to check if a container is alive or dead. If a liveness probe fails, the kubelet kills the container, and the container is subjected to its restart policy. If a container does not start after a failure, it is restarted again and again until it starts successfully or the kubelet kills the Pod.
    
  - Readiness probe: used to check if a container is ready to start accepting traffic. If a readiness probe fails, the endpoints controller removes the Pod's IP address from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of the service. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod. The Pod's IP address is also removed from the endpoints of all services that match the Pod.
    
  - Startup probe: used to check if a container has started. If a startup probe fails, the kubelet kills the container, and the container is subjected to its restart policy. If a container does not start after a failure, it is restarted again and again until it starts successfully or the kubelet kills the Pod.

  Probe types are mutually exclusive. If more than one is specified, the kubelet will ignore all but the first one.
   
## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](https://www.linkedin.com/feed/update/urn:li:share:7086718205188050945/)

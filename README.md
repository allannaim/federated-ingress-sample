# federated-ingress-sample

configmaps/zonefetch.yaml - retrieves the zone from the instance metadata server
and concatenates into volume mount path

replicasets/nginx-rs.yaml - deploys pods consisting of an nginx and busybox
container

ingress/ingress.yaml - creates a load balancer with a global VIP  that
distributes requests to the closest nginxzone backend

services/nginx.yaml - exposes the nginxzone backend as an external service



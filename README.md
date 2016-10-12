# federated-ingress-sample

configmaps/zonefetch.yaml - retrieves the zone from the instance metadata server
and concatenates into volume mount path

deployments/nginx-dep.yaml - deploys a pod consisting of an nginx and busybox
container

ingress/ingress.yaml - creates a load balancer with a global VIP  that
distributes requests to the closest nginxzone backend

services/nginxzone.yaml - exposes the nginxzone backend as an external service



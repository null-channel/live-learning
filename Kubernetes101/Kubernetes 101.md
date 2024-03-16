A working deployment. with two services that are networked together and exposed.

Topics:
 - deployment vs pod
 - configmpas
 - local k8s clusters

Learn about these tools:
- kubectl
- k9s

## Goals:
Learn Practical Kubernetes
- install kind and create cluster
	- cover other options (aka minikube, microk8s)
- REST app accessible outside cluster
	- should be configured using a configmap
	- should secret
		- talk about secure secrets
	- exposed via node port service
	- breakdown deployment/replicaset/pod
	- building our container?
- Using kubectl to exec into pod
- Use k9s and kubectl to view logs
- kubectl 
	- port forwarding
	- create local manifests
- deploy second app that talks to first
	- DNS
	- cluster ip
	- separate namespace
- understand and use labels
- leverage the scheduler (taints/tolortions)
	- make second app not run on the same node as first app.
- K8s in the cloud?


Future:
 - Kubernetes Networking
	 - CNI
	 - Ingress
	 - Service Mesh
	 - Network Policies
	 - Pain and suffering
 - Logging/Observability/tracing
 - Statefull workloads
 - CRDs/Operators
 - K8s on the cloud?

# Different components of Kubernetes

A Kubernetes cluster consists of a set of worker machines, called nodes, that run containerized applications. 
Every cluster has at least one worker node.


![img.png](img.png)






## Namespaces

In Kubernetes, namespaces provides a mechanism for isolating groups of resources within a single cluster. 
Names of resources need to be unique within a namespace, but not across namespaces. 
Namespace-based scoping is applicable only for namespaced objects (e.g. Deployments, Services, etc) and not for 
cluster-wide objects (e.g. StorageClass, Nodes, PersistentVolumes, etc).










# Deployment Yaml File

**Service** - The service acts as the load balancer. A load balancer is used to distribute requests
to the various available servers.

**Deployment** - Deployment will act as the intended application. The user request hits the load balancer, 
then the load balancer distributes the request by creating the number of replicas defined in the deployment.yaml file. 
For example, in our case, we have five replicas for scalability, meaning that we will have 5 instances running at a time.



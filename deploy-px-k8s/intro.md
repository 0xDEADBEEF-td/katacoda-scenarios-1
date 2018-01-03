[Portworx](https://portworx.com/) is a software defined persistent storage solution designed and purpose built for applications deployed as containers, via container orchestrators such as Kubernetes, Marathon and Swarm. It is a clustered block storage solution and provides a Cloud-Native layer from which containerized stateful applications programmatically consume block, file and object storage services directly through the scheduler.

In this tutorial, you will:

1. Learn how to deploy a 3 node Portworx Cluster.
2. Launch a `mysql` database and dynamically create a highly available PX volume.
3. Validate data persistence by killing a mysql instance.

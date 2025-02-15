## General Kubernetes Interview Questions

1. **What is Kubernetes and what are its main components?**
   - Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications. Its main components include the API server, etcd, controller manager, scheduler, and worker nodes.

2. **How does Kubernetes achieve high availability?**
   - Kubernetes achieves high availability through features like replication controllers, replica sets, and deployments which ensure that multiple instances of an application are running. It also uses health checks and automatic restarts to maintain application uptime.

3. **What is a Kubernetes Pod?**
   - A Pod is the smallest and simplest Kubernetes object. It represents a single instance of a running process in a cluster and can contain one or more containers that share the same network namespace and storage.

4. **Explain the concept of a Kubernetes Namespace.**
   - Namespaces in Kubernetes provide a way to divide cluster resources between multiple users. They are intended for use in environments with many users spread across multiple teams, or projects.

5. **What are Kubernetes Services and how do they work?**
   - Kubernetes Services are an abstraction that defines a logical set of Pods and a policy by which to access them. Services enable communication between different parts of an application and can be exposed internally or externally.

6. **How does Kubernetes handle scaling?**
   - Kubernetes handles scaling through Horizontal Pod Autoscaler (HPA) which automatically adjusts the number of Pods in a deployment based on observed CPU utilization or other select metrics.

7. **What is a Kubernetes Ingress and how is it used?**
   - An Ingress is a Kubernetes resource that manages external access to services within a cluster, typically HTTP. It provides load balancing, SSL termination, and name-based virtual hosting.

8. **Describe the role of etcd in Kubernetes.**
   - etcd is a distributed key-value store used by Kubernetes to store all cluster data, including configuration data, state data, and metadata. It is a critical component for maintaining the cluster's state and ensuring consistency.

9. **What is a ConfigMap in Kubernetes?**
   - A ConfigMap is a Kubernetes object used to store non-confidential configuration data in key-value pairs. It allows you to decouple configuration artifacts from image content to keep containerized applications portable.

10. **How do you perform a rolling update in Kubernetes?**
    - A rolling update in Kubernetes can be performed using the `kubectl rollout` command. This updates the Pods in a deployment incrementally, ensuring that some instances of the application are always available during the update process.
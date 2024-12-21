# Defination
...

    Kubernetes is an open source container orchestration engine for automating deployment, scaling, and management of containerized applications.
    Originally Developed by Google.
    The Open Source project is hosted by the Cloud Native Computing Foundation.
...
# Kubernetes Architecture
![Screenshot 2023-02-07 at 7 18 10 PM](https://kubernetes.io/images/docs/kubernetes-cluster-architecture.svg)
## Control plane Components
### kube-API Server
...

    The API Server is the frontend for the Kubernetes Control Plane.
    kube-API server is designed to scale horizontally—that is, it scales by deploying more instances.
    You can run several instances of kube-API server and balance traffic between those instances.
...
### etcd
...
     
      Its a distributed key value storage, which will store k8s cluster state.
      Cluster State - nummber of pods, their images, services etc

### kube-Scheduler
... 

    It Schedules the tasks/pods on the best fit worker node.
    The scheduler makes sure that which node is capable of handling the pod, deploys it on appropriate node.
### kube-Controller-manager
...

    is a key component of the Kubernetes control plane that runs controllers to handle routine tasks in the cluster.
    Controllers are processes that watch the state of your cluster, then make or request changes where needed.
### Cloud-Controller-manager
...

     The Cloud Controller Manager is a Kubernetes control plane component that embeds cloud-specific control logic.
     It allows Kubernetes to interact with cloud provider APIs, separating out the components that interact with the cloud platform from those that only interact with the cluster


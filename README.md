# ibmcloud-k8s
This is practice repo for IBM-Cloud-Kubernetes-service to refresh knowledge for deploying simple service.

## IBM Cloud Configuration
> If you're an IBMer then use following command
  ```shell
  ibmcloud login --sso
  ```
else
  ```shell
  ibmcloud login
  ```

## Kubernetes cluster setup on IBM Cloud

- Once you create a cluster then grab the `cluster-id` and run following command to connect with the IBM Cloud Kubernetes cluster.
  ```shell
  ibmcloud ks cluster config --{cluster-id}
  ```
- Once you are connected with the newly created kubernetes cluster then you can run following comment to see the existing list of the nodes.
  ```shell
  kubectl get nodes
  ```

- Point to the correct IBM Cloud Container Registry region.
  ```shell
  ibmcloud cr region-set us-south
  ```
- Create a unique namespace
  ```shell
  create that namespace <any_unique_namespace>
  ```
- Check current connected culster context using following command
  ```shell
  kubectl config current-context
  ```

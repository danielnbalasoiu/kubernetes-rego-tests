## Rego-based Audit for Kubernetes Resources

Examples of warnings generated by the policies in the `policy` folder:

```
WARN - Found service my-service of type LoadBalancer
WARN - The HTTPProxy server is a top-level proxy for server.fake-example.com
FAIL - The PersistentVolume data-nfs-server-provisioner-0 is mounting a hostpath
FAIL - The Pod task-pv-pod is mounting a hostpath
FAIL - bad-deployment must include Kubernetes recommended labels: https://kubernetes.io/docs/concepts/overview/working-with-objects/common-labels/#labels 
FAIL - bad-deployment in the Deployment ubuntu has an image, bad-deployment, using the latest tag
FAIL - bad-deployment in the Deployment bad-deployment does not have a memory limit set
FAIL - bad-deployment in the Deployment bad-deployment does not have a CPU limit set
FAIL - bad-deployment in the Deployment bad-deployment doesn't drop all capabilities
FAIL - bad-deployment in the Deployment bad-deployment is privileged
FAIL - bad-deployment in the Deployment bad-deployment is not using a read only root filesystem
FAIL - bad-deployment in the Deployment bad-deployment is running as root
FAIL - The Deployment bad-deployment is connected to the host network
FAIL - The Deployment bad-deployment is sharing the host PID
FAIL - The Deployment bad-deployment is mounting a hostpath
FAIL - Containers must not run as root in Deployment bad-deployment
FAIL - Deployment bad-deployment must provide app/release labels for pod selectors
```

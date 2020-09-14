# Authenticating inside the cluster

This example shows you how to configure a client with client-go to authenticate
to the Kubernetes API from an application running inside the Kubernetes cluster.

client-go uses the [Service Account token][sa] mounted inside the Pod at the
`/var/run/secrets/kubernetes.io/serviceaccount` path when the
`rest.InClusterConfig()` is used.

## Running this example

First install tile by following https://docs.tilt.dev/install.html

Then run the following command to launching application in your local k8s cluster.

```
tilt up
```
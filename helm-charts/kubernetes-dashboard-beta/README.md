# A Helm chart for deploying the kubernetes dashboard in the recommended way

This chart aims to replicate as much as possible the behaviour of running

```
$ kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0-rc3/aio/deploy/recommended.yaml
```

This chart provide however some extra features including deploying an ingress.

WARNING Exposing the dashboard outside the cluster is a bad idea, one way of
doing this safely would be to use an authenticating proxy.

Some information on using a oauth2_proxy can be found here:

https://blog.heptio.com/on-securing-the-kubernetes-dashboard-16b09b1b7aca

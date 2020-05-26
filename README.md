### Tail Sidecar

Use this for tailing the logs from main. This container has GNU core utils with GNU tail.
The following command will tail the log till it exists and exit gracefully
````tail --follow=name test.log````

This is a workaround for https://github.com/kubernetes/kubernetes/issues/25908

With Kubernetes 1.18 this can be solved by declaring the tailing container as sidecar
https://banzaicloud.com/blog/k8s-sidecars/


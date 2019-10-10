SERVICE:::

>kubectl expose deployment hello-world --type=NodePort --name=example-service

>kubectl describe services example-service



PODS RUNNING WITH THIS SELECTOR:::
>kubectl get pods --selector="run=load-balancer-example" --output=wide


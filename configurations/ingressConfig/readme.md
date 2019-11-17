Using K8s Ingress on kind and exposing ports
------------------------------------------------------------------------------------------------------------------
$ kubectl apply -f https://raw.githubusercontent.com/ernestojballon/kubernetes/master/configurations/ingressConfig/mandatory.yml

$ kubectl apply -f https://raw.githubusercontent.com/ernestojballon/kubernetes/master/configurations/ingressConfig/cloud-generic.yaml

Now we have an Ingress controller (hooray), but how can we access it? Let’s check the external IP of the Ingress Service that NGINX created:

$ kubectl get services -n ingress-nginx
NAME            TYPE           CLUSTER-IP      EXTERNAL-IP   PORT(S)                      AGE
ingress-nginx   LoadBalancer   10.106.112.12   <pending>     80:32293/TCP,443:32117/TCP   16m

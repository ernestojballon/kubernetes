Using K8s Ingress on kind and exposing ports
------------------------------------------------------------------------------------------------------------------
$ kubectl apply -f https://raw.githubusercontent.com/ernestojballon/kubernetes/master/configurations/ingressConfig/mandatory.yml

$ kubectl apply -f https://raw.githubusercontent.com/ernestojballon/kubernetes/master/configurations/ingressConfig/cloud-generic.yaml

Now we have an Ingress controller (hooray), but how can we access it? Let’s check the external IP of the Ingress Service that NGINX created:

$ kubectl get services -n ingress-nginx


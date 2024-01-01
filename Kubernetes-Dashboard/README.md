# Steps:
1. Enable dashboard using `minikube addons enable dashboard`. This will create kubernetes dashboard service. 
2. Note the IP address and Port number of the enabled service using `kubectl get svc -n kubernetes-dashboard`
3. Add host-name and corresponding IP address of kubernetes-dashboard in /etc/hosts file.
4. Run `kubectl apply -f dashboard-ingress.yaml` to create ingress component.
5. Now, kubernetes dashboard can be accessed at the address `dashboard2.com`
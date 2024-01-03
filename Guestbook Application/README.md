## Deploying PHP Guestbook application with Redis

### Objectives: 
0. Start Minikube cluster using `minikube start --vm-driver={hyperv name}`
1. Start up a redis leader.
\
`kubectl apply -f redis-leader-deployment.yaml`
2. Start up two redis followers.
\
`kubectl apply -f redis-follower-deployment.yaml`
3. Start up the guestbook frontend.
\
`kubectl apply -f guestbook-frontend-deployment.yaml`
4. Expose and view the Frontend Service using 
\
`minikube service {svc-name}`
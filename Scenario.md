# Kubernetes_advanced-webapp
...and some helm



**********-----------------------------------**********
Hi there, this was a university project.

 We did nearly the whole thing before with docker and docker-compose(also in my repo). 
 We got the exercise (graded) to do the whole thing with kubernetes this time and as an
 addition the database deployment with helm charts(no usage of templates).

 I had to anonymize all the names of applications and the sources of the images
 due to being the official dockerhub repo of the university. 
 

Cheers

**********-----------------------------------**********

used:
- mircok8s
- kubectl
- ubuntu server 18.04 lts

Kubernetes Exercise:
- Ingress on Port 80, no cert
- 1 namespace for ui-/web-tier
- 1 namespace for database
- 3 pods for ui-tier, at least 1 running when deployment getrs reapplied and new pods are being made
- 1 pod for backend, gets killed before new pod before reapplied deployment pod gets created
- configmaps for database location used
- secrets configured (yaml) and created (console) (make sure you encrypt your strings first with md5)

Helm:
- deployment of database within own database namespace

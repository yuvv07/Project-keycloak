# Project-keycloak

What is keycloak ?
Keycloak is an Open Source Identity and Access Management(IAM) Software, which will act as an essential tool in your business product. IAM typically aims to verify the identity of a user or system which is requesting access to your environment, and evaluates a set of rules which tells what features and assets is that user/system has access to.
- Hello Guys! In this project I have deployed a Open Source IAM tool in my local environment with Kubernetes.
- I have used minikube kubernetes cluster.
- First I have created a yaml file in which a POD and a Service is created, go through the keycloak.yaml.
- Apply/Run this file.
- kubectl apply -f keycloak.yml
- As you can see a Service with LoadBalancer type is created from which the keycloak console can be access from outside the cluster itself.
- Then, a POD is created with mention of Ports, Image, Arguments and Environment, In env we are creating a user, admin and its password who will be accessing console for the first time.
- Enter the minikube cluster and curl to minikube's ip to check if keycloak is working.
- if you check Service External IP isn't available yet, for that Run service or easy option Run a minikube tunnel in separate terminal, it will provide a external ip.
- Go to the browser type ip with port number, There you Go! it will be working just fine login through admin credentials.

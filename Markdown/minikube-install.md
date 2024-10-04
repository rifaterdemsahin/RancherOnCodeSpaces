sudo apt-get update -y
sudo apt-get install -y apt-transport-https
curl -Lo minikube https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube /usr/local/bin/


E1004 18:00:47.373526   30614 status.go:263] The "minikube" host does not exist!
minikube
type: Control Plane
host: Nonexistent
kubelet: Nonexistent
apiserver: Nonexistent
kubeconfig: Nonexistent

@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ minikube status
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured

@rifaterdemsahin ➜ /workspaces/RancherOnCodeSpaces (main) $ 


minikube start --driver=docker

kubectl create deployment helloworld --image=nginx

kubectl expose deployment helloworld --type=NodePort --port=80

minikube service helloworld --url

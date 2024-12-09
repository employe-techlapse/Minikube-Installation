# Minikube-Installation

# Steps:-
sudo apt-get update
sudo apt-get install docker.io -y
sudo usermod -aG docker $USER && newgrp docker

curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube 

****************************************************************************************************************************************
curl (Client URL) is a command-line tool used to transfer data to or from a server. It supports a wide range of protocols, including 
HTTP, HTTPS, FTP, FTPS, SCP, SFTP, TFTP, LDAP, POP3, IMAP, SMTP, GOPHER,
****************************************************************************************************************************************

sudo snap install kubectl --classic
minikube start --driver=docker

# Reboot your machine once using below command
# sudo reboot
# minikube service --url svcname
# kubectl get po -o wide -n web-app
# minikube ssh
# curl http://10.244.0.3:5000
# svcname.namspace.svc.cluster.local
# kubectl describe service my-lb -n web-app
# sudo fuser -k 80/tcp
# netstat -tunlp

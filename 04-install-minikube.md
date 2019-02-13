# Step 1: Update system
```
sudo apt-get update

sudo apt-get install apt-transport-https

sudo apt-get upgrade
```
# Step 2: Install KVM or VirtualBox Hypervisor
```
sudo apt install virtualbox virtualbox-ext-pack
```
# Step 3: Download minikube
```javascript
wget https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

chmod +x minikube-linux-amd64

sudo mv minikube-linux-amd64 /usr/local/bin/minikube
```

# Step 4: Install kubectl on Ubuntu 18.04

```
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
```

* Add Kubernetes apt repository:

```
echo "deb http://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list
```
* Update apt index and install kubectl
```
sudo apt update
sudo apt -y install kubectl
```
* Check version:

```
kubectl version -o json 
```
# Step 5: Starting minikube
```
minikube start
```
# Step 6: Minikube Basic operations
```
kubectl cluster-info
```
---
title: "minikube start"
source: "https://minikube.sigs.k8s.io/docs/start/?arch=%2Flinux%2Fx86-64%2Fstable%2Fbinary+download"
author:
  - "[[minikube]]"
published:
created: 2025-11-16
description: "minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes.All you need is Docker (or similarly compatible) container or a Virtual Machine environment, and Kubernetes is a single command away: minikube startWhat you’ll need 2 CPUs or more 2GB of free memory 20GB of free disk space Internet connection Container or virtual machine manager, such as: Docker, QEMU, Hyperkit, Hyper-V, KVM, Parallels, Podman, VirtualBox, or VMware Fusion/Workstation 1Installation Click on the buttons that describe your target platform. For other architectures, see the release page for a complete list of minikube binaries."
tags:
  - "clippings"
---
minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes.

All you need is Docker (or similarly compatible) container or a Virtual Machine environment, and Kubernetes is a single command away: `minikube start`

## What you’ll need

- 2 CPUs or more
- 2GB of free memory
- 20GB of free disk space
- Internet connection
- Container or virtual machine manager, such as: [Docker](https://minikube.sigs.k8s.io/docs/drivers/docker/), [QEMU](https://minikube.sigs.k8s.io/docs/drivers/qemu/), [Hyperkit](https://minikube.sigs.k8s.io/docs/drivers/hyperkit/), [Hyper-V](https://minikube.sigs.k8s.io/docs/drivers/hyperv/), [KVM](https://minikube.sigs.k8s.io/docs/drivers/kvm2/), [Parallels](https://minikube.sigs.k8s.io/docs/drivers/parallels/), [Podman](https://minikube.sigs.k8s.io/docs/drivers/podman/), [VirtualBox](https://minikube.sigs.k8s.io/docs/drivers/virtualbox/), or [VMware Fusion/Workstation](https://minikube.sigs.k8s.io/docs/drivers/vmware/)

## 1Installation

Click on the buttons that describe your target platform. For other architectures, see [the release page](https://github.com/kubernetes/minikube/releases/latest) for a complete list of minikube binaries.

Operating system

Architecture

Release type

Installer type

Installer type

Release type

Installer type

Installer type

Release type

Installer type

Installer type

Release type

Installer type

Installer type

Release type

Installer type

Installer type

Architecture

Release type

Installer type

Installer type

Release type

Installer type

Installer type

Architecture

Release type

Installer type

Installer type

To install the latest minikube **stable** release on **x86-64** **Linux** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64
```

To install the latest minikube **beta** release on **x86-64** **Linux** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-linux-amd64' | head -n1)
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64
```

To install the latest minikube **stable** release on **x86-64** **Linux** using **Debian package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
sudo dpkg -i minikube_latest_amd64.deb
```

To install the latest minikube **beta** release on **x86-64** **Linux** using **Debian package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube_.*_amd64.deb' | head -n1)
curl -L $u > minikube_beta_amd64.deb && sudo dpkg -i minikube_beta_amd64.deb
```

To install the latest minikube **stable** release on **x86-64** **Linux** using **RPM package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.x86_64.rpm
sudo rpm -Uvh minikube-latest.x86_64.rpm
```

To install the latest minikube **beta** release on **x86-64** **Linux** using **RPM package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-.*.x86_64.rpm' | head -n1)
curl -L $u > minikube-beta.x86_64.rpm && sudo rpm -Uvh minikube-beta.x86_64.rpm
```

To install the latest minikube **stable** release on **ARM64** **Linux** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-arm64
sudo install minikube-linux-arm64 /usr/local/bin/minikube && rm minikube-linux-arm64
```

To install the latest minikube **beta** release on **ARM64** **Linux** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-linux-arm64' | head -n1)
sudo install minikube-linux-arm64 /usr/local/bin/minikube && rm minikube-linux-arm64
```

To install the latest minikube **stable** release on **ARM64** **Linux** using **Debian package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_arm64.deb
sudo dpkg -i minikube_latest_arm64.deb
```

To install the latest minikube **beta** release on **ARM64** **Linux** using **Debian package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube_.*_arm64.deb' | head -n1)
curl -L $u > minikube_beta_arm64.deb && sudo dpkg -i minikube_beta_arm64.deb
```

To install the latest minikube **stable** release on **ARM64** **Linux** using **RPM package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.aarch64.rpm
sudo rpm -Uvh minikube-latest.aarch64.rpm
```

To install the latest minikube **beta** release on **ARM64** **Linux** using **RPM package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-.*.aarch64.rpm' | head -n1)
curl -L $u > minikube-beta.aarch64.rpm && sudo rpm -Uvh minikube-beta.aarch64.rpm
```

To install the latest minikube **stable** release on **ppc64** **Linux** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-ppc64le
sudo install minikube-linux-ppc64le /usr/local/bin/minikube && rm minikube-linux-ppc64le
```

To install the latest minikube **beta** release on **ppc64** **Linux** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-linux-ppc64le' | head -n1)
sudo install minikube-linux-ppc64le /usr/local/bin/minikube && rm minikube-linux-ppc64le
```

To install the latest minikube **stable** release on **ppc64** **Linux** using **Debian package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_ppc64le.deb
sudo dpkg -i minikube_latest_ppc64le.deb
```

To install the latest minikube **beta** release on **ppc64** **Linux** using **Debian package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube_.*_ppc64le.deb' | head -n1)
curl -L $u > minikube_beta_ppc64le.deb && sudo dpkg -i minikube_beta_ppc64le.deb
```

To install the latest minikube **stable** release on **ppc64** **Linux** using **RPM package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.ppc64el.rpm
sudo rpm -Uvh minikube-latest.ppc64el.rpm
```

To install the latest minikube **beta** release on **ppc64** **Linux** using **RPM package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-.*.ppc64el.rpm' | head -n1)
curl -L $u > minikube-beta.ppc64el.rpm && sudo rpm -Uvh minikube-beta.ppc64el.rpm
```

To install the latest minikube **stable** release on **S390x** **Linux** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-s390x
sudo install minikube-linux-s390x /usr/local/bin/minikube && rm minikube-linux-s390x
```

To install the latest minikube **beta** release on **S390x** **Linux** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-linux-s390x' | head -n1)
sudo install minikube-linux-s390x /usr/local/bin/minikube && rm minikube-linux-s390x
```

To install the latest minikube **stable** release on **S390x** **Linux** using **Debian package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_s390x.deb
sudo dpkg -i minikube_latest_s390x.deb
```

To install the latest minikube **beta** release on **S390x** **Linux** using **Debian package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube_.*_s390x.deb' | head -n1)
curl -L $u > minikube_beta_s390x.deb && sudo dpkg -i minikube_beta_s390x.deb
```

To install the latest minikube **stable** release on **S390x** **Linux** using **RPM package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.s390x.rpm
sudo rpm -Uvh minikube-latest.s390x.rpm
```

To install the latest minikube **beta** release on **S390x** **Linux** using **RPM package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-.*.s390x.rpm' | head -n1)
curl -L $u > minikube-beta.s390x.rpm && sudo rpm -Uvh minikube-beta.s390x.rpm
```

To install the latest minikube **stable** release on **ARMv7** **Linux** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-linux-arm
sudo install minikube-linux-arm /usr/local/bin/minikube && rm minikube-linux-arm
```

To install the latest minikube **beta** release on **ARMv7** **Linux** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-linux-arm' | head -n1)
sudo install minikube-linux-arm /usr/local/bin/minikube && rm minikube-linux-arm
```

To install the latest minikube **stable** release on **ARMv7** **Linux** using **Debian package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_armhf.deb
sudo dpkg -i minikube_latest_armhf.deb
```

To install the latest minikube **beta** release on **ARMv7** **Linux** using **Debian package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube_.*_armhf.deb' | head -n1)
curl -L $u > minikube_beta_armhf.deb && sudo dpkg -i minikube_beta_armhf.deb
```

To install the latest minikube **stable** release on **ARMv7** **Linux** using **RPM package**:

```shell
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-latest.armv7hl.rpm
sudo rpm -Uvh minikube-latest.armv7hl.rpm
```

To install the latest minikube **beta** release on **ARMv7** **Linux** using **RPM package**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
u=$(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-.*.armv7hl.rpm' | head -n1)
curl -L $u > minikube-beta.armv7hl.rpm && sudo rpm -Uvh minikube-beta.armv7hl.rpm
```

To install the latest minikube **stable** release on **x86-64** **macOS** using **Homebrew**:

If the [Homebrew Package Manager](https://brew.sh/) is installed:

```shell
brew install minikube
```

If `which minikube` fails after installation via brew, you may have to remove the old minikube links and link the newly installed binary:

```shell
brew unlink minikube
brew link minikube
```

To install the latest minikube **stable** release on **x86-64** **macOS** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-darwin-amd64
sudo install minikube-darwin-amd64 /usr/local/bin/minikube
```

To install the latest minikube **beta** release on **x86-64** **macOS** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-darwin-amd64' | head -n1)
sudo install minikube-darwin-amd64 /usr/local/bin/minikube
```

To install the latest minikube **stable** release on **ARM64** **macOS** using **binary download**:

```shell
curl -LO https://github.com/kubernetes/minikube/releases/latest/download/minikube-darwin-arm64
sudo install minikube-darwin-arm64 /usr/local/bin/minikube
```

To install the latest minikube **stable** release on **ARM64** **macOS** using **Homebrew**:

If the [Homebrew Package Manager](https://brew.sh/) is installed:

```shell
brew install minikube
```

If `which minikube` fails after installation via brew, you may have to remove the old minikube links and link the newly installed binary:

```shell
brew unlink minikube
brew link minikube
```

To install the latest minikube **beta** release on **ARM64** **macOS** using **binary download**:

```shell
r=https://api.github.com/repos/kubernetes/minikube/releases
curl -LO $(curl -s $r | grep -o 'http.*download/v.*beta.*/minikube-darwin-arm64' | head -n1)
sudo install minikube-darwin-arm64 /usr/local/bin/minikube
```

To install the latest minikube **stable** release on **x86-64** **Windows** using **Windows Package Manager**:

If the [Windows Package Manager](https://docs.microsoft.com/en-us/windows/package-manager/) is installed, use the following command to install minikube:

```shell
winget install Kubernetes.minikube
```

To install the latest minikube **stable** release on **x86-64** **Windows** using **Chocolatey**:

If the [Chocolatey Package Manager](https://chocolatey.org/) is installed, use the following command:

```shell
choco install minikube
```

To install the latest minikube **stable** release on **x86-64** **Windows** using **.exe download**:

1. Download and run the installer for the [latest release](https://storage.googleapis.com/minikube/releases/latest/minikube-installer.exe).  
	Or if using `PowerShell`, use this command:
	```powershell
	New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force
	$ProgressPreference = 'SilentlyContinue'; Invoke-WebRequest -OutFile 'c:\minikube\minikube.exe' -Uri 'https://github.com/kubernetes/minikube/releases/latest/download/minikube-windows-amd64.exe' -UseBasicParsing
	```
2. Add the `minikube.exe` binary to your `PATH`.  
	*Make sure to run PowerShell as Administrator.*
	```powershell
	$oldPath = [Environment]::GetEnvironmentVariable('Path', [EnvironmentVariableTarget]::Machine)
	if ($oldPath.Split(';') -inotcontains 'C:\minikube'){
	  [Environment]::SetEnvironmentVariable('Path', $('{0};C:\minikube' -f $oldPath), [EnvironmentVariableTarget]::Machine)
	}
	```
	If you used a terminal (like powershell) for the installation, please close the terminal and reopen it before running minikube.

To install the latest minikube **beta** release on **x86-64** **Windows** using **.exe download**:

1. Download and run the installer for the [latest beta release](https://github.com/kubernetes/minikube/releases/download/v1.33.0-beta.0/minikube-installer.exe).  
	Or if using `PowerShell`, use this command:
	```powershell
	New-Item -Path 'c:\' -Name 'minikube' -ItemType Directory -Force
	$response = Invoke-WebRequest -Uri 'https://api.github.com/repos/kubernetes/minikube/releases' -UseBasicParsing
	$json = $response.Content | ConvertFrom-Json
	$item = ($json | ?{ $_.prerelease -eq $true })[0].assets | ?{ $_.name -eq 'minikube-windows-amd64.exe' }
	Invoke-WebRequest -Uri $item.browser_download_url -OutFile 'c:\minikube\minikube.exe' -UseBasicParsing
	```
2. Add the `minikube.exe` binary to your `PATH`.  
	*Make sure to run PowerShell as Administrator.*
	```powershell
	$oldPath = [Environment]::GetEnvironmentVariable('Path', [EnvironmentVariableTarget]::Machine)
	if ($oldPath.Split(';') -inotcontains 'C:\minikube'){
	  [Environment]::SetEnvironmentVariable('Path', $('{0};C:\minikube' -f $oldPath), [EnvironmentVariableTarget]::Machine)
	}
	```
	*If you used a CLI to perform the installation, you will need to close that CLI and open a new one before proceeding.*

## 2Start your cluster

From a terminal with administrator access (but not logged in as root), run:

```shell
minikube start
```

If minikube fails to start, see the [drivers page](https://minikube.sigs.k8s.io/docs/drivers/) for help setting up a compatible container or virtual-machine manager.

## 3Interact with your cluster

If you already have kubectl installed (see [documentation](https://kubernetes.io/docs/tasks/tools/install-kubectl/)), you can now use it to access your shiny new cluster:

```shell
kubectl get po -A
```

Alternatively, minikube can download the appropriate version of kubectl and you should be able to use it like this:

```shell
minikube kubectl -- get po -A
```

You can also make your life easier by adding the following to your shell config: (for more details see: [kubectl](https://minikube.sigs.k8s.io/docs/handbook/kubectl/))

```shell
alias kubectl="minikube kubectl --"
```

Initially, some services such as the storage-provisioner, may not yet be in a Running state. This is a normal condition during cluster bring-up, and will resolve itself momentarily. For additional insight into your cluster state, minikube bundles the Kubernetes Dashboard, allowing you to get easily acclimated to your new environment:

```shell
minikube dashboard
```

## 4Deploy applications

Create a sample deployment and expose it on port 8080:

```shell
kubectl create deployment hello-minikube --image=kicbase/echo-server:1.0
kubectl expose deployment hello-minikube --type=NodePort --port=8080
```

It may take a moment, but your deployment will soon show up when you run:

```shell
kubectl get services hello-minikube
```

The easiest way to access this service is to let minikube launch a web browser for you:

```shell
minikube service hello-minikube
```

Alternatively, use kubectl to forward the port:

```shell
kubectl port-forward service/hello-minikube 7080:8080
```

Tada! Your application is now available at [http://localhost:7080/](http://localhost:7080/).

You should be able to see the request metadata in the application output. Try changing the path of the request and observe the changes. Similarly, you can do a POST request and observe the body show up in the output.

To access a LoadBalancer deployment, use the “minikube tunnel” command. Here is an example deployment:

```shell
kubectl create deployment balanced --image=kicbase/echo-server:1.0
kubectl expose deployment balanced --type=LoadBalancer --port=8080
```

In another window, start the tunnel to create a routable IP for the ‘balanced’ deployment:

```shell
minikube tunnel
```

To find the routable IP, run this command and examine the `EXTERNAL-IP` column:

```shell
kubectl get services balanced
```

Your deployment is now available at <EXTERNAL-IP>:8080

Enable ingress addon:

```shell
minikube addons enable ingress
```

The following example creates simple echo-server services and an Ingress object to route to these services.

```shell
kind: Pod
apiVersion: v1
metadata:
  name: foo-app
  labels:
    app: foo
spec:
  containers:
    - name: foo-app
      image: 'kicbase/echo-server:1.0'
---
kind: Service
apiVersion: v1
metadata:
  name: foo-service
spec:
  selector:
    app: foo
  ports:
    - port: 8080
---
kind: Pod
apiVersion: v1
metadata:
  name: bar-app
  labels:
    app: bar
spec:
  containers:
    - name: bar-app
      image: 'kicbase/echo-server:1.0'
---
kind: Service
apiVersion: v1
metadata:
  name: bar-service
spec:
  selector:
    app: bar
  ports:
    - port: 8080
---
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: example-ingress
spec:
  rules:
    - http:
        paths:
          - pathType: Prefix
            path: /foo
            backend:
              service:
                name: foo-service
                port:
                  number: 8080
          - pathType: Prefix
            path: /bar
            backend:
              service:
                name: bar-service
                port:
                  number: 8080
---
```

Apply the contents

```shell
kubectl apply -f https://storage.googleapis.com/minikube-site-examples/ingress-example.yaml
```

Wait for ingress address

```shell
kubectl get ingress
NAME              CLASS   HOSTS   ADDRESS          PORTS   AGE
example-ingress   nginx   *       <your_ip_here>   80      5m45s
```

**Note for Docker Desktop Users:**  
To get ingress to work you’ll need to open a new terminal window and run `minikube tunnel` and in the following step use `127.0.0.1` in place of `<ip_from_above>`.

Now verify that the ingress works

```shell
$ curl <ip_from_above>/foo
Request served by foo-app
...

$ curl <ip_from_above>/bar
Request served by bar-app
...
```

## 5Manage your cluster

Pause Kubernetes without impacting deployed applications:

```shell
minikube pause
```

Unpause a paused instance:

```shell
minikube unpause
```

Halt the cluster:

```shell
minikube stop
```

Change the default memory limit (requires a restart):

```shell
minikube config set memory 9001
```

Browse the catalog of easily installed Kubernetes services:

```shell
minikube addons list
```

Create a second cluster running an older Kubernetes release:

```shell
minikube start -p aged --kubernetes-version=v1.34.0
```

Delete all of the minikube clusters:

```shell
minikube delete --all
```
- [The minikube handbook](https://minikube.sigs.k8s.io/docs/handbook/)
- [Community-contributed tutorials](https://minikube.sigs.k8s.io/docs/tutorials/)
- [minikube command reference](https://minikube.sigs.k8s.io/docs/commands/)
- [Contributors guide](https://minikube.sigs.k8s.io/docs/contrib/)
- Take our [fast 5-question survey](https://forms.gle/Gg3hG5ZySw8c1C24A) to share your thoughts 🙏

---

  

Last modified September 2, 2025: [Update Kubernetes versions (ce0ab0036)](https://github.com/kubernetes/minikube/commit/ce0ab003608e00fd868941ed02a835e21158493a)
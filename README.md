# starting docker in rootless mode with minikube, kubectl, containerd, & qemu

what you will need to have installed before you start:<br>
*docker<br>
*dockerd-rootless-setuptool.sh<br>
*minikube<br>
*kubectl<br>
*qemu-system-x86<br>

To get started with docker using containerd as the runtime and qemu as the runtime:<br>

"<b><h6>dockerd-rootless-setuptool.sh install<br>
export DOCKER_HOST=unix:///run/user/1000/docker.sock<br>
minikube start --container-runtime=containerd --driver=qemu2<br>
DOCKER_HOST=unix:///run/user/1000/docker.sock kubectl get pods</h6></b>"<br>
<br>
<br>
<br>

https://docs.docker.com/engine/security/rootless/

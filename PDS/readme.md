# Access Minikube NodePort Service via SSH Tunnel

This guide explains how to access a Kubernetes service running in **Minikube on a remote server** from your local machine using SSH port forwarding.

---

## SSH Command

```bash
ssh -i devops-assignment-prajwal -o GatewayPorts=true prajwal@35.200.207.110 -N -f -L 8000:192.168.49.2:30007


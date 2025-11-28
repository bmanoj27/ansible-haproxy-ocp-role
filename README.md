# ansible-role-haproxy-ocp-lb

An Ansible role to install and configure HAProxy as a load balancer for OpenShift UPI clusters.

## Features
- Installs HAProxy
- Configures Kubernetes API load balancing
- Configures Machine Config Server load balancing
- Configures Ingress HTTP/HTTPS load balancing
- Dynamic master/worker lists

## Usage

Modify the defaults/main.yaml to have your own hostnames and IP addresses.

```yaml
- hosts: haproxy
  roles:
    - haproxy-ocp-lb

1. Playbook for site

2. If Failing
    1. Check that all machines have the same name for network interface

    2. Check if the K8 api server is up and accessible for example: curl -kv https://10.0.0.222:6443 and 10.0.0.11

    3. Make sure metalLB and kube api server have the proper IP's

    4. Manually set the virtual IP for control nodes

    5. Hail marry, reset playbook

3. Install Cilium CLI for interaction | [install](https://docs.cilium.io/en/stable/gettingstarted/k8s-install-default/)

4. Set config for exclusive CNI to false | `cilium config set cni-exclusive false` [source](https://github.com/istio/istio/issues/46764)



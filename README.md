# Helm Chart to deploy Workadventure

This is a Helm Chart to deploy [WorkAdventure](https://github.com/thecodingmachine/workadventure)

Based on work done by gmoirod in repository [gmoirod/helm-workadventure](https://github.com/gmoirod/helm-workadventure).


## Deployment on a Giantswarm Workload Cluster

- Install nginx-ingress-controller-app and cert-manager-app (already installed on AWS)
- Make a copy of [`sample-values/gs-cluster.yaml`](sample-values/gs-cluster.yaml)
- Edit your values file to match your desired configuration
- Install this app using your values
- Wait until pods are up and certificates have been issued, access your instance by navigating to `https://play.$yourdomain(configured in your values.yaml)`.

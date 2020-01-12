# helm-wordpress :circus_tent:

Repository mit Helm Chart für Wordpress mit MySQL :smirk:

# Prerequists

Folgende CustomResourceDefinitions sind zwingend notwendig und müssen vorab manuell installiert werden:

- templates/customResourceDefinitions.yaml

```sh
$ kubectl apply -f ./templates/customResourceDefinitions.yaml
```

# Lokale Bash-History für Stable Wordpress Helm Chart als Vorlage

```sh
$ helm repo add stable https://kubernetes-charts.storage.googleapis.com/
$ helm search repo wordpress
$ helm repo update
$ helm help
$ mkdir stable
$ cd stable
$ helm pull stable/wordpress
$ helm install -h
$ helm create test
$ helm install . --dry-run --debug --generate-name --skip-crds
```
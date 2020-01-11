# helm-wordpress :circus_tent:

Repository mit Helm Chart für lesetraum.blog :smirk:

# Lokale Bash-History für Stable Wordpress Helm Chart als Vorlage
helm repo add stable https://kubernetes-charts.storage.googleapis.com/
helm search repo wordpress
helm repo update
helm help
mkdir stable
cd stable
helm pull stable/wordpress
helm install -h

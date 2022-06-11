# Create Node-exporter
kubectl create -f  node-exporter.yaml


# Create Prometheus
kubectl create -f rbac-setup.yaml

kubectl create -f configmap.yaml

kubectl create -f prometheus.pvc.yaml

kubectl create -f prometheus.deploy.yaml

kubectl create -f prometheus.svc.yaml


# Create Grefana
kubectl create -f grafana-pvc.yaml

kubectl create -f grafana-deploy.yaml 

kubectl create -f grafana-svc.yaml

kubectl create -f grafana-ing.yaml 


# mysql-prometheus-grafana
Kubernetes deployment contains MySQL, Prometheus and Grafana.

#### Clone the repo:
git clone git@github.com:ganasubrgit/mysql-prometheus-grafana.git

#### change dir
cd mysql-prometheus-grafana

#### Deploy using Kubectl 
kubectl apply -f deployment.yaml 

#### Port forward for prometheus your local laptop/desktop
kubectl port-forward <pod name> -n monitoring 9090:9090
use browser http://localhost:9090/ 

#### Port forward for grafana your local laptop/desktop
kubectl port-forward <pod name> -n monitoring 3000:3000
http://localhost:3000/

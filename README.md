Установка Prometheus+Grafana:
```bash
  helm install stack prometheus-community/kube-prometheus-stack -f prometheus/prometheus.yaml
```
Установка ingress-nginx:
```bash
  helm install ingress-otus ingress-nginx/ingress-nginx -f prometheus/nginx-ingress.yaml
```
Установка приложения:
```bash
  helm install otus . -f values.yaml
```
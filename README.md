# helm-charts-testing
Charts de Helm para pruebas del Centro Gestor.

Para la instalación se requiere un cluster de kubernetes y el gestor de paquetes Helm.

## Agregar los repositorios de Helm

```bash
helm repo add energetica2030 https://github.com/Energetica2030/helm-charts-testing

helm repo add bitnami https://charts.bitnami.com/bitnami
helm repo update
```
## Instalar los charts de Helm
### Apache Kafka

```bash
helm install kafka bitnami/kafka
```

### Servicio de reporte de inercia
```bash
helm install inertia-service energetica2030/inertia-service
```

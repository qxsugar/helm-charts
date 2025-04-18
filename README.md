# webhookx

Helm chart installation for the open-source project webhookx.

## Dependencies

| Repository                         | Name       | Version |
|------------------------------------|------------|---------|
| https://charts.bitnami.com/bitnami | postgresql | 6       |
| https://charts.bitnami.com/bitnami | redis      | 17      |

## Install Dependencies

1. helm repo add bitnami https://charts.bitnami.com/bitnami
2. helm repo update
3. helm install postgresql --namespace webhookx --create-namespace bitnami/postgresql
4. helm install redis --namespace webhookx --create-namespace bitnami/redis

## Install webhookx

1. helm repo add webhookx https://webhookx.github.io/helm-charts
2. helm repo update
3. helm install webhookx webhookx/webhookx --namespace webhookx --create-namespace

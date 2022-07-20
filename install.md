# Kyverno

## Kyverno

```shell
helm repo add kyverno https://kyverno.github.io/kyverno/
helm repo update
```

```shell
helm install kyverno-policies kyverno/kyverno-policies -n kyverno --create-namespace
```

## Policy Reporter

```shell
helm repo add policy-reporter https://kyverno.github.io/policy-reporter
helm repo update
```

```shell
helm install policy-reporter policy-reporter/policy-reporter -n policy-reporter --set metrics.enabled=true --set rest.enabled=true --create-namespace
```

## Policy Reporter UI

```shell
helm repo add policy-reporter https://kyverno.github.io/policy-reporter
helm repo update
```

```shell
helm upgrade --install policy-reporter policy-reporter/policy-reporter --create-namespace -n policy-reporter --set ui.enabled=true

```

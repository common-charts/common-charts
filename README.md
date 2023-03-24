# helm commons charts

## Usage

[Helm](https://helm.sh) must be installed to use the charts.
Please refer to Helm's [documentation](https://helm.sh/docs/) to get started.

Once Helm is set up properly, add the repo as follows:

```bash
helm repo add common-charts https://common-charts.github.io/common-charts/
helm repo list
```

You can then run `helm search repo common-charts` to see the charts.

### install
```bash
helm install my-nginx common-charts/web -n default
```

# create a helm chart

## step 1

```bash
mkdir charts
cd charts
helm create web
```

## 更新依赖
```
cd charts/web
helm dependency update
```

## lint

```
cd charts/web
helm lint --strict
```

## 模拟测试
```
cd charts/web
helm template . | more
```

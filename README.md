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

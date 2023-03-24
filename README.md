# helm commons charts

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

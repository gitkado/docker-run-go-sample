# docker-run-go-sample

### 標準パッケージのみで実行

```sh
docker run --rm -v $PWD:/go golang:latest go run sample.go
```

### 標準パッケージ以外に必要な場合（Dockerfile追記必要）

```sh
docker build -t go-dev .
docker run --rm -v $PWD:/go go-dev:latest go run sample.go
```

### Dockerfile のイメージを使う
```bash
$ docker build -t my_php ./docker
$ docker image ls
```

### サーバー起動
```bash
$ docker run --rm \
  --publish 8000:8000 \
  --name php-container \
  --volume $(pwd):/myapp \
  my_php -t /myapp -S 0.0.0.0:8000
```

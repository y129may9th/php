# サーバー起動
```bash
$ docker run --rm \
  --publish 8000:8000 \
  --name php-image
  --volume $(pwd):/myapp 
  php -t /myapp -S 0.0.0.0:8000
```

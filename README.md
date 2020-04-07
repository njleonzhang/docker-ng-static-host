# mp-docker-static-host

image of nginx in docker for host static spa website

## build image and push to repository
```
docker build . -t t-docker-hub.meipian.cn/fore/mp-docker-static-host:0.0.1

docker push t-docker-hub.meipian.cn/fore/mp-docker-static-host
```

## use image
just copy static file to ng folder

```
FROM t-docker-hub.meipian.cn/fore/mp-docker-static-host:0.0.1
COPY view/index.html /var/www/html/   // 将目标文件 copy 到 ng 目录下。
```
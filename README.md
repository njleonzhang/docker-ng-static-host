# mp-docker-spa-host

image of nginx in docker for host static spa website

## build image and push to repository
```
docker build . -t t-docker-hub.meipian.cn/fore/mp-docker-spa-host:0.0.1

docker push t-docker-hub.meipian.cn/fore/mp-docker-spa-host
```

## use image
write a docker file in the project,

```
FROM t-docker-hub.meipian.cn/fore/mp-docker-spa-host:0.0.1
COPY view/index.html /var/www/html/   // 将目标文件 copy 到 ng 目录下。
```
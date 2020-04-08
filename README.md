# docker-ng-static-host

image of nginx in docker for host static spa website

## use image
just copy static file to ng folder

```
FROM njleonzhang/ng-static-host
COPY view/index.html /var/www/html/   // 将目标文件 copy 到 ng 目录下。
```

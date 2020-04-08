# docker-nginx-spa-host

docker image for hosting static spa website by nginx

## features
* redirect requests to `index.html` for support spa history mode
* empty response to `/listen` `GET` request for health check.

## Use image

```
FROM njleonzhang/nginx-spa-host
COPY view/index.html /var/www/html/  // copy your index.html to nginx folder.
```


# docker-ng-static-host

image of nginx in docker for host static spa website

* redirect requests to `index.html` for support spa history mode
* empty response to `/listen` `GET` request for health check.

## Use image
just copy static file to ng folder

```
FROM njleonzhang/ng-static-host
COPY view/index.html /var/www/html/  // copy your index.html to nginx folder.
```


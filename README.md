## A simple static page for testing browser capability


#### Prerequisite

1. Install node.js and [http-server npm module](https://www.npmjs.com/package/http-server)


#### Generate self-signed cert and key

```
$> openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./self.key -out ./self.crt
```


#### Run in HTTP

```
$> http-server
```


#### Run in HTTPS

```
$> http-server --ssl --cert ./self.crt --key ./self.key
```


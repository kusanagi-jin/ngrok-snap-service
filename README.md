# ngrok-snap-service

1. ngrok-auth token
2. edit $HOME/snap/ngrok-snap-service/current/.ngrok/ngrok.yml

expects

```yaml
authtoken: xxx
region: eu
log_level: info
log_format: json
tunnels:
  http:
    addr: 80
    proto: http
    hostname: yourdomain.com
    bind_tls: false
  https:
    addr: 443
    proto: tls
    hostname: yourdomain.com
```

https://github.com/snapcore/action-publish

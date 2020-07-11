# ngrok-service

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/ngrok-service)

or install via `snap install ./ngrok-service_2.3.35_all.snap --dangerous`

edit $HOME/snap/ngrok-snap-service/current/.ngrok/ngrok.yml

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

published via https://github.com/snapcore/action-publish

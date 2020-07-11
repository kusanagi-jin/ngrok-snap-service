# ngrok-service

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/ngrok-service)

or install via

```sh
snap install ./ngrok-service_2.3.35_all.snap --dangerous
snap ngrok-auth your-ngrok-auth-token
# edit $HOME/snap/ngrok-service/current/.ngrok/ngrok.yml
snap start ngrok-service.http
snap start ngrok-service.https

systemctl status snap.ngrok-service.ngrok-service-https.service

```

expects

```yaml
authtoken: xxx
region: eu
log_level: info
log_format: json
tunnels:
  app-http:
    addr: 80
    proto: http
    hostname: yourdomain.com
    bind_tls: false
  app-https:
    addr: 443
    proto: tls
    hostname: yourdomain.com
```

published via https://github.com/snapcore/action-publish

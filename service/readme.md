### reverse proxy

```bash
docker run -d --rm -it -p 7999:7999 --name=ninja \
  -e WORKERS=1 \
  -e LOG=info \
  gngpp/ninja:latest run -D
```

### enable docker daemon

```bash
sudo service docker start # for SysVinit
sudo systemctl start docker # for Systemd
```
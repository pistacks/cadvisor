# cadvisor
cAdvisor for ARM

## Version

- pistacks/cadvisor:0.34.0

## Usage

```
docker run \
  --volume=/:/rootfs:ro \
  --volume=/var/run:/var/run:ro \
  --volume=/sys:/sys:ro \
  --volume=/var/lib/docker/:/var/lib/docker:ro \
  --volume=/dev/disk/:/dev/disk:ro \
  --publish=8080:8080 \
  --detach=true \
  --name=cadvisor \
  pistacks/cadvisor:0.34.0
```

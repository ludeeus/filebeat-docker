# filebeat-docker

_Filebeat for docker._

```bash
docker run --name filebeat -d \
  -e EKHOST='192.168.2.110' \
  -v /var/run/docker.sock:/var/run/docker.sock:ro \
  -v /var/lib/docker/containers/:/var/lib/docker/containers/:ro \
  ludeeus/filebeat-docker:dev
```
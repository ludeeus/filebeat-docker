# filebeat-docker

_Filebeat for docker._

```bash
docker run --name filebeat \
  -e EKHOST='192.168.2.110' \
  -v /var/run/docker.sock:/var/run/docker.sock \
  ludeeus/filebeat-docker
```
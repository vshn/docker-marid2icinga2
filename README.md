# docker-marid2icinga2 - OpsGenie marid in docker

Run a OpsGenie marid daemon inside docker, prepared for icinga2 integration.
Also see: https://docs.opsgenie.com/v1.0/docs/icinga2-integration

## Logging
* All logging goes to the console (you can use `docker logs` now)

## Configuration
Unfortunately configuration is still done by mounting the configuration file.

## Example Run
Running as non-root is not yet supported.
```
docker run -v /etc/opsgenie/marid_docker/instance-vshn.conf:/etc/opsgenie/conf/opsgenie-integration.conf vshn/marid2icinga2
```

## Known-issues
* cannot run as non-root yet
* configuration via environment variables not possible yet

## Credit
https://github.com/davidkarlsen/docker-marid

# Phobos Third Party Integration Infrastructure

![Phobos™ logo](/docs/images/phobos_logo.png)

This repository contains sets of [`docker-compose`](https://docs.docker.com/compose/overview/) files used to help [Phobos](https://phobos.petabridge.com/) users evaluate the [third party monitoring and tracing integrations supported by Phobos](https://phobos.petabridge.com/articles/integrations.html).

These Docker files are __not intended for production use__. They are meant for evaluation purposes only. 

## Monitoring Infrastructure
* [StatsD + Grafana](monitoring/statsd)

## Tracing Infrastructure
* [Zipkin](tracing/zipkin)

## License
Phobos is a commercial product and [its end-user license agreement can be found here](https://phobos.petabridge.com/articles/setup/license.html).

The sources in this repository, however, is open source and is [licensed under the terms of Apache 2.0](LICENSE).

This library is maintained by [Petabridge](https://petabridge.com/)®. Copyright 2015-2018.
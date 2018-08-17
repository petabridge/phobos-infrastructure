# Zipkin
This `docker-compose` file is originally from the [OpenZipkin organization's official Docker files](https://github.com/openzipkin/docker-zipkin), and we encourage users interested in testing [Phobos.Tracing's Zipkin integration](https://phobos.petabridge.com/articles/tracing/backends/zipkin.html).

## Setup
To run this image, clone this repository and set your current working directory to this folder.

Once there and provided that you have Docker installed on your system, run the following command:

```
PS> docker-compose up -d
```

This will spin up three Docker containers:

1. Zipkin, whose port will be exposed on http://localhost:9411. This is the value you will want to use inside the `phobos.tracing.zipkin.http.uri` setting in order to actually gather data from Phobos. It is also the URI of the web UI where you can view the traces collected.
2. MySQL, the backing store used by Zipkin in this instance for storing relevant trace data. And
3. Zipkin-Dependencies, an Apache Spark job running in the background that stitches all of the traces together for the Zipkin UI.
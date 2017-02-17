
[![Docker Automated build](https://img.shields.io/docker/automated/itzg/thrift.svg)](https://hub.docker.com/r/itzg/thrift)

This image just provides a pre-built Apache Thrift generator tool.

Within the container the entrypoint, `thrift`, runs in the working directory
`/home`, so the recommended usage is:

```
docker run -v $(pwd):/home thrift --gen [language] [file]
```

which would result in a `gen-[language]` directory populated in your current
host directory.

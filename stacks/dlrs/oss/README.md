## Deep Learning Reference Stack with Optimized Eigen

[![](https://images.microbadger.com/badges/image/clearlinux/stacks-dlrs-oss.svg)](http://microbadger.com/images/clearlinux/stacks-dlrs-oss "Get your own image badge on microbadger.com")

### Building Locally

Default build args in Docker are on: https://docs.docker.com/engine/reference/builder/#arg

```
docker build --no-cache -t clearlinux/stacks-dlrs-oss .
```

### Optional Build ARGs

* `swupd_args` specifies [swupd update](https://github.com/clearlinux/swupd-client/blob/master/docs/swupd.1.rst#options) flags passed to the update during build.

>NOTE: An empty `swupd_args` will default to Clear Linux OS latest version. Consider this when building from the Dockerfile, as an OS update will be performed. The docker image in this registry was built and validated using version 28680.

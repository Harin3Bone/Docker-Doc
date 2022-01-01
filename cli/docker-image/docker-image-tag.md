---
description: Tag image
---

# docker image tag

### Synopsis

```
docker image tag
```

### Options

None of options

### Commands

* Tag image

```
docker image tag <source> <target>
```

> :notebook\_with\_decorative\_cover: **Note**
>
> `<source>` is your reference **image name** or **image id**
>
> `<target>` is new image name by your tag

_Example_

```
docker image tag redis:latest asia.gcr.io.redis:latest
```

also you can use

```
docker tag <source> <target>
```

_Example_

```
docker tag redis:latest asia.gcr.io.redis:latest
```

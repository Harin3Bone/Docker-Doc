---
description: Remove one or more images
---

# docker image rm

### Synopsis

```
docker image rm
```

### Options

* \-f
* \--force
  * Force remove image
* \--no-prune
  * Do not delete untagged parent

### Commands

* Remove image

```
docker image rm <value>
```

```
docker rmi <value>
```

> :notebook\_with\_decorative\_cover: **Note**
>
> `<value>` is a **image id** or **image name:version**

* Remove all image

```
docker image rm $(docker image ls -a)
```

```
docker rmi $(docker images -a)
```

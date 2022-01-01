---
description: List image
---

# docker image ls

### Synopsis

```
docker image ls
```

### Options

* \-a
* \--all
  * Show all images
* \--digests
  * Show digests
* \-f
* \--filter
  * Filter output based on conditions provided
* \--format
  * Pretty-print images using `Go` template
* \--no-trunc
  * Do not truncate output
* \-q
* \--quite
  * Only show image ID

### Commands

* List image

```
docker image ls
```

```
docker images
```

* List all image

```
docker image ls -a
```

```
docker images -a
```

* List only image id

```
docker image ls -q
```

```
docker images -q
```

> :notebook\_with\_decorative\_cover: **Note**
>
> You can combine with `-a` or `--all` like this too
>
> ```
> docker images -a -q
> ```

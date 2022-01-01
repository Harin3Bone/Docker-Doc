# docker run

### Synopsis

```
docker run
```

### Options

* \--add-host
  * Add a custom host to IP mapping

> :notebook\_with\_decorative\_cover: **Note**
>
> Mapping by `host`:`ip`

* \-a
  * Attach to `STDIN` , `STDOUT` or `STDERR`
* \--cpus
  * Number of **CPUs**
* \--cpuset-mems
  * **MEMs** in which to allow execution
* \-d
  * Run container in background and print container ID
* \--device
  * Add a host device to the container
* \--dns
  * Set custom **DNS Server**
* \--dns-opt
  * Set **DNS** options
* \--entrypoint
  * Overwrite the default `ENTRYPOINT` of the image
* \-e
  * Set environment variables
* \--env-file
  * Read in a file of environment variables
* \--expose
  * Expose a port or a range of ports
* \--gpus
  * **GPU** device to add to the container

> :notebook\_with\_decorative\_cover: **Note**
>
> Set **all** to pass all **GPUs**

* \-h
  * Container host name
* \--health-cmd
  * Command to run to check health
* \--health-interval
  * Time between running check
* \--health-retries
  * Consecutive failures needed to report unhealthy
* \--health-start-period
  * Start period for the container to initialize before starting `health-retires` countdown
* \--health-timeout
  * Maximum time to allow one check to run

> :notebook\_with\_decorative\_cover: **Note**
>
> Time unit of `--health-interval` , `--health-start-period` and `--health-timeout` include
>
> 1. ms = milliseconds
> 2. s = seconds
> 3. m = minutes
> 4. h = hours
>
> **Default value is 0s**

* \--init
  * Run an init inside the container
* \-i
  * Keep `STDIN` open even if not attached
* \--isolation
  * Container isolation technology
* \--io-maxbandwidth
  * Maximum **IO bandwidth** limit for system drive
* \--io-maxiops
  * Maximum **IOps** limit for the system drive

> :notebook\_with\_decorative\_cover: **Note**
>
> `--io-maxbandwidth` and `--io-maxiops` are allow to use in **Windows** only

* \--ip
  * Set IPv4 address
* \--ip6
  * Set IPv6 address
* \--ipc
  * Use IPC mode

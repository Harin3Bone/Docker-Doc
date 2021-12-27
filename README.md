---
description: This content make for whoever want to learn about Docker from basic.
---

# Docker

![Reference: https://www.docker.com/company/newsroom/media-resources](.gitbook/assets/horizontal-logo-monochromatic-white.png)

### What is Docker ?

Docker is an open platform for developing, shipping and running applications. Docker enables you to separate your applications from your infrastructure.

### Why we use Docker ?

We can delivery software quickly with Docker and manage infrastructure in the same ways you manage your applications. By taking advantage of Docker methodologies for shipping, testing and deploying code quickly.

### Installation

Docker can installed in Windows, MacOS and Linux

{% tabs %}
{% tab title="Windows" %}
1. Install **WSL** by Microsoft documentation from this [link](https://docs.microsoft.com/en-us/windows/wsl/install)
2. Download from this [link](https://docs.docker.com/desktop/windows/install/)
3. Run Docker installer
{% endtab %}

{% tab title="MacOS" %}
1. Download from this [link](https://docs.docker.com/desktop/mac/install/)
2. Run `Docker.dmg`
3. Drag the Docker icon to the Application folder
4. Run `Docker.app` in the Applications folder
{% endtab %}

{% tab title="Linux" %}
**Debian/Ubuntu**

1\. Update the `apt` package and allow `apt` to use HTTPS

```
sudo apt-get update

sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

2\. Add Docker official GPG Keys

```
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

3\. Setup stable repository

```
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

4\. Install Docker Engine

```
sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io
```

5\. Verify that Docker Engine is installed correctly

```
docker --version
```
{% endtab %}
{% endtabs %}

### Post Installation (Linux)

Commonly when docker install finished it can access as **root** user only. Because of that I recommended everyone do this for make docker can access by non-root user

1\. Create the **docker** group

```
sudo groupadd docker
```

2\. Add your user to the **docker** group

```
sudo usermod -aG docker $USER
```

3\. Logout and Login so that your group membership is re-evaluated

```
newgrp docker
```

4\. Verify that you can run **docker** command without `sudo`

```
docker run hello-world
```

### Configure Docker to start on boot (Linux)

Most current Linux are use `systemd` to manage which services start when the system boots. On **Debian** and **Ubuntu** the docker service are configured to start on boot by default. To automatically start Docker and Container on boot for other distro use command below.

```
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
```

To disable this behavior, use `disable` instead.

```
sudo systemctl disable docker.service
sudo systemctl disable containerd.service
```

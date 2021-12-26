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
4. Run `Docker.app` in the Applications folder&#x20;
{% endtab %}

{% tab title="Linux" %}
ddssDebian/Ubuntu

1. Update the `apt` package and allow `apt` to use HTTPS

```
sudo apt-get update

sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release
```

1. Add Docker official GPG Keys

```
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

1. Setup stable repository

```
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

1. Install Docker Engine

```
sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io
```

1. Verify that Docker Engine is installed correctly

```
docker --version
```
{% endtab %}
{% endtabs %}


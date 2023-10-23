# Vorbereitung Server

## Installation Docker

Die einfachste Möglichkeit, den Minetest-Server lokal laufen zu lassen, ist der fertige Docker-Container.

### Installation Docker Linux / Ubuntu

Auf der Seite von Docker wird die Installation Schritt für Schritt erklärt:

{% embed url="https://docs.docker.com/engine/install/ubuntu/" %}
Anleitung zur Installation von Docker
{% endembed %}

#### [Install using the apt repository](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository)

Before you install Docker Engine for the first time on a new host machine, you need to set up the Docker repository. Afterward, you can install and update Docker from the repository.

1.  Set up Docker's `apt` repository.

    ```bash
    # Add Docker's official GPG key:
    sudo apt-get update
    sudo apt-get install ca-certificates curl gnupg
    sudo install -m 0755 -d /etc/apt/keyrings
    curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
    sudo chmod a+r /etc/apt/keyrings/docker.gpg

    # Add the repository to Apt sources:
    echo \
      "deb [arch="$(dpkg --print-architecture)" signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
      "$(. /etc/os-release && echo "$VERSION_CODENAME")" stable" | \
      sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
    sudo apt-get update
    ```

    > **Note**
    >
    > If you use an Ubuntu derivative distro, such as Linux Mint, you may need to use `UBUNTU_CODENAME` instead of `VERSION_CODENAME`.
2. Install the Docker packages.
3.  ***

    To install the latest version, run:

    ```console
    $ sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
    ```

    ***
4.  Verify that the Docker Engine installation is successful by running the `hello-world` image.

    ```console
    $ sudo docker run hello-world
    ```

    This command downloads a test image and runs it in a container. When the container runs, it prints a confirmation message and exits.

You have now successfully installed and started Docker Engine.

### Weitere benötigte Pakete

Du benötigst noch:

* GIT
* Python3
* PIP

Unter Ubuntu kannst Du diese Pakete mit folgendem Befehl installieren:

```bash
sudo apt install python3 python3-pip git
```

Um die Karten in Minetest zu generieren, das heißt anhand der Koordinatien aus OpenStreetMap zu exportieren und eine entsprechende Vorlage in Minetest zu generieren werden zusätzlich folgende Python-Module benötigt:

```bash
sudo apt install python3-pyproj python3-numpy python3-tqdm python3-matplotlib
```

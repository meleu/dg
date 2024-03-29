---
{"dg-publish":true,"permalink":"/notes/learning/docker-mastery/docker-installation-udemy/"}
---

## Installation

- back to [[notes/learning/docker-mastery/Docker Mastery - udemy\|Docker Mastery - udemy]]

> [!NOTE]
> I wrote this while doing the [[notes/learning/docker-mastery/Docker Mastery - udemy\|Docker Mastery - udemy]] course. For installing docker I suggest to follow the steps in the official documentation.

```sh
sudo apt-get remove docker docker-engine docker.io containerd runc

# the script below does NOT work with Linux Mint :(
# detailed instructions here: https://docs.docker.com/get-docker/

curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh

sudo usermod -aG docker meleu

# just checking:
docker version
```

- Install `docker-machine`: <https://github.com/docker/machine/releases/>

- Install `docker-compose`: <https://docs.docker.com/compose/install/>

Clone de course repository:
```sh
git clone https://github.com/bretfisher/udemy-docker-mastery
```

Install VS Code **and the Docker plugin**.

Bonus: check also [SpaceVim](https://spacevim.org/).


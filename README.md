# pyenv-test-container

A simple Dockerized Ubuntu developer environments with some basic tools installed that helps developers to create a portable debugging solution.

## List of tools installed

- [oh-my-zsh](https://ohmyz.sh/)
- [pyenv](https://github.com/pyenv/pyenv)

## How to use

Run the following commands to build the environment then start the container:

```bash
chmod +x setup.sh
./setup.sh
```

Then you can use the container by running the following command:

```bash
docker run -p 8888:8888 -v ${PWD}:/home/root/app --rm auto-setup-pyenv jupyter notebook --allow-root --ip=0.0.0.0 app
```

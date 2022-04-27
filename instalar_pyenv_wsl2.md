## Instalar pyenv no wsl2

```
curl https://pyenv.run | bash

sudo apt-get update; sudo apt-get install make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```
## Coloque as linhas a seguir no arquivo ~/.bashrc e reinicie o seu terminal
```
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

export PIPENV_VENV_IN_PROJECT=enabled
```

## A partir de então para instalar versões do python em seu wsl2 basta usar o comando

```bash
#Instalar python versão 3.10.4
pyenv install 3.10.4

#Instalar python 3.9.6
pyenv install 3.9.6

#Listar todas as versões diponíveis para instalar
pyenv install -l
```
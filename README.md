# Docker Container - svn2git
---

[![Build Status](http://drone.vertigo.com.br/api/badges/docker/svn2git/status.svg)](http://drone.vertigo.com.br/docker/svn2git)
[![](https://badge.imagelayers.io/vertigo/svn2git:latest.svg)](https://imagelayers.io/?images=vertigo/svn2git:latest 'Get your own badge on imagelayers.io')

A minimalist container to use the (awesome) svn2git tool.

## Modo de usar
---

Caso o repositório SVN se encontre na estrutura padrão de SVN (/trunk, /tags e /branches), basta executar os comandos abaixo.

```bash
$ mkdir pasta-destino-do-projeto
```

```bash
$ docker run -it -v $(pwd)/pasta-destino-do-projeto:/svn2git vertigobr/svn2git [REPOSITÓRIO]
```

Caso deseje incluir o nome de cada usuário que fez o commit no projeto, tenha um arquivo texto na seguinte forma:

  username-no-svn = Nome do Usuário <email-no-git@vertigo.com.br>
  username2-no-svn = Nome do Usuário2 <email2-no-git@vertigo.com.br>

```bash
$ docker run -it -v $(pwd)/pasta-destino-do-projeto:/svn2git -v $(pwd)/authors.txt:/authors.txt vertigobr/svn2git --authors /authors.txt [REPOSITÓRIO]
```
---

Documentação do svn2git [aqui](https://github.com/nirvdrum/svn2git)

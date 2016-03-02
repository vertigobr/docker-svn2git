# Docker Container - svn2git
---

[![Build Status](http://drone.vertigo.com.br/api/badges/docker/svn2git/status.svg)](http://drone.vertigo.com.br/docker/svn2git)
[![](https://badge.imagelayers.io/vertigo/svn2git:latest.svg)](https://imagelayers.io/?images=vertigo/svn2git:latest 'Get your own badge on imagelayers.io')

A minimalist container to use the (awesome) svn2git tool.

## Modo de usar
---


```bash
$ mkdir pasta-destino-do-projeto
```

```bash
$ cd pasta-destino-do-projeto
```

```bash
$ docker run -it -v $(pwd):/svn2git vertigobr/svn2git [COMANDO_SVN2GIT]
```
---

Documentação do svn2git [aqui](https://github.com/nirvdrum/svn2git)

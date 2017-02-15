# Git

---

GitHub es una plataforma de desarrollo colaborativo para alojar proyectos utilizando el sistema de control de versiones Git. Se llama control de versiones a la gestion de diversos cambios que se realizan sobre los elementos de algún producto o una configuración del mismo. Una version, revision o edicion de un producto, es el estado en el que se encuentra el mismo en un momento dado de su desarrollo![](/assets/Git-logo.svg).

![](/assets/Captura de pantalla 2017-02-15 a las 19.31.40.png)

> Credits: Wikipedia

### Instalación de Git en Linux

* Para distribuciones Fedora, RedHat y CentOS

```markdown
$ yum install git-core
```

* Para distribuciones Debian y Ubuntu

```markdown
$ apt-get install git-core
```

### Configuración

Antes de empezar a utilizar Git, es recomendable dedicar un par de minutos a establecer algunas opciones de configuracion utiles. Estas opciones se establecen mediante el comando _git config_. En primer lugar, define tu nombre y email de contacto ejecutando los siguientes comandos:

```markdown
$ git config --global user.name "Javier Eguiluz"
$ git config --global user.email javier.eguiluz@gmail.com
```

## Guia de comandos Git

> Credits: rogerdudler.github.io

### Add & commit

* Crear un repositorio

```
$ git init
```

* Clonar repositorio

```markdown
$ git clone <ruta>
```

* Registrar cambios 

```markdown
$ git add <filename>
$ git add .
```

* Hacer commit a dichos cambios

```markdown
$ git commit -m "Commit message"
```

### Envío de cambios y ramas

* Para el envío de cambios al repositorio remoto

```markdown
$ git push origin master
```

* Para crear una rama

```markdown
$ git branch <nombre_rama>
```

* Para moverse a una rama

```markdown
$ git checkout <nombre_rama>
```

### Actualizar y fusionar

* Para actualizar el repositorio local al commit más nuevo

```markdown
$ git pull
```

* Para fusionar otra rama a tu rama activa

```markdown
$ git merge <branch>
```

* Para fusionar otra rama con tu rama activa y borrarla \(se añade como commit\)

```markdown
$ git rebase <branch>
```




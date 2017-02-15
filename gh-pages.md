## ![](/assets/Captura de pantalla 2017-02-15 a las 19.36.17.png)

---

## Que son las gh-pages

Las gh-pages o _Github pages_ son páginas web que Github pone a nuestra disposición para nuestros proyectos, con la particularidad de que estas deben de estar alojadas en los repositorios propios de Github. Con el simple gesto de actualizar nuestro repositorio, también estaremos haciendo lo propio con la gh-page.

Para crear una Github Page haremos lo siguiente:

1. Crear un repositorio en GitHub con nombre _nombredeusuario.\_github.io, donde \_nombredeusuario_ es tu nombre de usuario o nombre de organización. El nombre es importante ya que si no, no funcionará el link principal.
2. Clona el repositorio que has creado para trabajar sobre el y comenzar tu proyecto.
3. Crea un index.html si quieres trabajar en HTML. En nuestro caso utilizaremos Markdown, por lo que nuestra pagina se llama index.md.
4. Add, commit y push para comenzar con tu GitHub page.

## Como usar el módulo _gh-pages_

El módulo gh-pages te permite automatizar el despliegue en GitHub Pages. Para instalarlo correctamente haremos lo siguiente:

```markdown
$ gitbook init librodeprueba
$ cd librodeprueba/
$ gitbook build
$ npm init -yes
$ npm install gh-pages --save
```

Esto te crea un libro de prueba, sobre el que hemos inicializado npm y hemos instalado el módulo gh-pages. Para crear un \_deploy \_que ejecute el módulo, utilizaremos el siguiente script:

```markdown
var ghpages = require('gh-pages');
var path = require('path');
ghpages.publish(path.join(__dirname,'_book'),function(err){
    console.log('publicado en gh-pages'+err);
});
```




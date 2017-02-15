# ![](/assets/Captura de pantalla 2017-02-15 a las 19.34.29.png)

---

> Credits: Pandoc.org

Si necesitas convertir archivos desde un formato de marcas a otro, pandoc es lo que necesitas. Puede convertir documentos en [markdown](http://daringfireball.net/projects/markdown/), [reStructuredText](http://docutils.sourceforge.net/docs/ref/rst/introduction.html), [textile](http://redcloth.org/textile), [HTML](http://www.w3.org/TR/html40/), [DocBook](http://www.docbook.org/), [LaTeX](http://www.latex-project.org/), [MediaWiki markup](http://www.mediawiki.org/wiki/Help:Formatting), [TWiki markup](http://twiki.org/cgi-bin/view/TWiki/TextFormattingRules), [OPML](http://dev.opml.org/spec2.html), Emacs [Org-Mode](http://orgmode.org/), [Txt2Tags](http://txt2tags.org/), Microsoft Word [docx](http://www.microsoft.com/interop/openup/openxml/default.aspx), LibreOffice [ODT](http://en.wikipedia.org/wiki/OpenDocument), [EPUB](http://en.wikipedia.org/wiki/EPUB), o [Haddock markup](http://www.haskell.org/haddock/doc/html/ch03s08.html) a:

* Formatos HTML
* Formatos Word
* Ebooks
* Formatos de documentación

### Instalando pandoc

Pandoc provee de un instalador para Debian, Ubuntu, Mac y Windows en el siguiente enlace: [https://github.com/jgm/pandoc/releases/tag/1.19.2.1](https://github.com/jgm/pandoc/releases/tag/1.19.2.1)

### Comandos de pandoc

Estos comandos te permiten convertir un fichero de entrada en un fichero HTML:

* Fragmento HTML:

```markdown
$ pandoc MANUAL.txt -o example1.html
```

* Archivo HTML estandar:

```markdown
$ pandoc -s MANUAL.txt -o example2.html
```

* HTML con CSS:

```markdown
$ pandoc -s -S --toc -c pandoc.css -A footer.html MANUAL.txt -o example3.html
```




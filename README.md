# CSS3

## Introducción a CSS

CSS es el acrónimo de _**"Cascading Style Sheets"**_, que significa **Hojas de Estilo en Cascada**. Es el lenguaje utilizado para dar estilo y formato a un documento HTML. CSS describe como los elementos deben renderizarse en una pantalla, en un hoja impresa o cualquier otro medio.

Se le denomina **en cascada** porque se lee, procesa y aplica el código desde arriba hacia abajo.

Anteriormente, el desarrollo de varias partes de la especificación CSS se hizo de forma paralela, lo que permitió que hubiera una versión de las últimas recomendaciones como por ejemplo CSS1, CSS2.1, o incluso CSS3.

**Nunca habrá una versión CSS4**. Más bien, todo es ahora código CSS sin un número de versión ya que CSS se divide en módulos independientes que se desarrollan a diferente ritmo.

Las especificaciones de CSS se encuentran en [W3C specifications](https://www.w3.org/Style/CSS/#specs).

## Integrar CSS

### Estilos integrados en un elemento HTML

La regla CSS se aplica directamente sobre el elemento HTML. De esta forma la regla **sólo** se aplica al elemento HTML y no puede reutilizarse:

```html
<p>Lorem <span style="color: red; padding: 8px">ipsum dolor</span></p>
```

### Estilos definidos en el documento HTML

Las reglas CSS se definen en un documento HTML. Por tanto se aplican a **todo** el documento HTML únicamente. Se utiliza la etiqueta `<style>` dentro de la etiqueta `<head>`:

```html
<!DOCTYPE html>
<html>
<head>
  <title>...</title>
  <style>
    div {
      background: red;
      color: white;
    }
  </style>
</head>
  ...
</html>
```

### Estilos definidos en un archivo CSS externo

Las reglas CSS se definen en un **archivo CSS externo**. Estas reglas se podrán reutilizar en todos los documentos HTML que incluyan el archivo CSS.

:warning: El atributo `type="text/css"` es opcional ya que el tipo de las hojas de estilo por defecto es CSS.

```html
<!DOCTYPE html>
<html>
<head>
  <title>...</title>
  <link rel="stylesheet" href="index.css" />
</head>
  ...
</html>
```

### Estilos importados

Una forma de integrar una hoja de estilo CSS es utilizar la regla `@import`, regla implementada en CSS2.

Esta regla permite importar una hoja de estilo CSS **dentro** de otra hoja de estilo CSS.

```css
/* index.css */
@import url("otra-hoja.css")
```

También se puede utilizar dentro de un documento HTML aunque por rendimiento este método no es recomendable:

```html
<!DOCTYPE html>
<html>
<head>
  <title>...</title>
  <style>
    @import url("otra-hoja.css");
  </style>
</head>
  ...
</html>
```

---

## Enlaces de interés

- <https://lenguajecss.com/css/>
- <https://www.w3.org/Style/CSS/>
- <https://www.w3.org/Style/CSS/specs.en.html>
- <https://developer.mozilla.org/en-US/docs/Web/CSS>
- <https://web.dev/learn/css?hl=es>
- <https://htmlcheatsheet.com/css/>
- <https://overapi.com/css>
- <https://cheatsheets.shecodes.io/css>
- <https://cssreference.io/>
- <https://www.w3schools.com/css/>
- <https://devhints.io/>
- <https://www.theodinproject.com/>
- <https://roadmap.sh/frontend>
- <https://jsfiddle.net>

## Licencia

[![Licencia de Creative Commons](https://i.creativecommons.org/l/by-sa/4.0/80x15.png)](http://creativecommons.org/licenses/by-sa/4.0/)
Esta obra está bajo una [licencia de Creative Commons Reconocimiento-Compartir Igual 4.0 Internacional](http://creativecommons.org/licenses/by-sa/4.0/).

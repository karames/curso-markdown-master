# Código fuente

## Código fuente en línea

- Inserción en línea de la sintaxis o palabra que pertenezca a código fuente.
- Empezar y terminar con 1 acento grave.

```markdown
- Texto normal `sintaxis código fuente` y aquí continua el texto.
```

- Texto normal `sintaxis código fuente` y aquí continua el texto.

### Ejemplos código fuente en línea

```markdown
- El salto de línea en **HTML** se consigue con la etiqueta `<br>` y aquí continua el texto.
- La estructua condicional en **JavaScript** es del tipo `if...else...endif` y aquí continua.
```

- El salto de línea en **HTML** se consigue con la etiqueta `<br>` y aquí continua el texto.
- La estructua condicional en **JavaScript** es del tipo `if...else...endif` y aquí continua.

## Código fuente en bloque

- Inserción de un bloque de código fuente.
- Empezar y terminar con 3 acentos graves, especificando el lenguaje al principio (se usa para resaltar con colores los elementos).
- También se puede utilizar 3 ~ (virgulilla) al principio y al final (no recomendable).

````markdown
```lenguaje
código fuente
```
````

### Ejemplos código fuente en bloque

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Título de la página</title>
  </head>
  <body></body>
</html>
```

```javascript
function transitionEnd() {
  var el = document.createElement("bootstrap");

  var transEndEventNames = {
    WebkitTransition: "webkitTransitionEnd",
    MozTransition: "transitionend",
    OTransition: "oTransitionEnd otransitionend",
    transition: "transitionend",
  };

  for (var name in transEndEventNames) {
    if (el.style[name] !== undefined) {
      return { end: transEndEventNames[name] };
    }
  }

  return false; // explicit for ie8 (  ._.)
}
```

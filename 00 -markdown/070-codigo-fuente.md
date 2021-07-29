# Código fuente

## Uso

- Permite mostrar código fuente en un documento markdown.

## Sintaxis

- Empezar y terminar con 3 acentos graves, especificando el lenguaje al principio (se usa para resaltar con colores los elementos).

```lenguaje
código fuente
```

</pre>

## Ejemplos

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

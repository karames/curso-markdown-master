# Imágenes

- Inserción de imágenes.
- Sintaxis igual que los enlaces, pero anteponiendo el carácter \! al principio.

```markdown
![texto alt imagen](url "etiqueta")
```

- Parámetros:
  - texto alt imagen: texto alternativo de la imagen si no se encuentra.
  - url: dirección de la imagen (absoluta o relativa).
  - "etiqueta": es opcional y muestra tooltip con información sobre la imagen.

## Ejemplo inserción imágenes

```markdown
![Imagen Batman existe](/images/batman.png "Batman")
![Imagen Batman no existe](/images/batman0.png "Batman")
```

![Imagen Batman existe](/images/batman.png "Batman")
![Imagen Batman no existe](/images/batman0.png "Batman")

## Imágenes con referencia o marcador

- Si existen varias imágenes se puede colocar entre corchetes una numeración a modo de marcador para vincular la imagen al final del contenido del documento.

```markdown
![texto alt imagen][referencia]
...
...
...
Al final del documento:
[referencia]: url "etiqueta"
```

- Parámetros:
  - texto alt imagen: texto alternativo de la imagen si no se encuentra.
  - referencia: marcador utilizado como referencia en la imagen
  - url: dirección de la imagen (absoluta o relativa).
  - "etiqueta": es opcional y muestra tooltip con información sobre la imagen.

### Ejemplo imágenes con referencia

```markdown
![Imagen Capitán América][imagen capitan america]
![Imagen Superman][imagen superman]
...
...
...
Al final del documento:
[imagen capitan america]: /images/capitan-america.png "Capitán América"
[imagen superman]: /images/superman.png "Superman"
```

![Imagen Capitán América][imgcapitanamerica]
![Imagen Superman][imgsuperman]

[imgcapitanamerica]: /images/capitan-america.png "Capitán América"
[imgsuperman]: /images/superman.png "Superman"

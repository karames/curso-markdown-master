# Enlaces

## Enlaces normales

- Inserción de enlaces a recursos.
- Sintaxis:

```markdown
[texto del recurso](url "etiqueta")
```

- Parámetros:
  - texto del recurso: texto del enlace.
  - url: dirección del recurso (absoluta o relativa).
  - "etiqueta": es opcional y muestra tooltip con información sobre el enlace.

### Ejemplo enlaces normales

```markdown
- [Enlace a Google](https://www.google.es/ "Ir a Google")
- [Karames Formacion](https://formacion.karames.es/ "Ir a Plataforma de Formación")
```

- [Enlace a Google](https://www.google.es/ "Ir a Google")
- [Karames Formacion](https://formacion.karames.es/ "Ir a Plataforma de Formación")

## Enlaces con referencia o marcador

- Desventajas enlaces normales:
  - En general, dificultan la lecturas del documento, problema que se agrava si las direcciones son largas o complejas.
  - Si es un mismo enlace aparece varias veces, entonces es necesario repetirlo tantas veces como aparezca.
- Solución -> enlaces con referencia:
  - Permiten solucionar los problemas anteriores.
  - Permite una mejor organización del documento.

### Sintaxis

```markdown
[texto del recurso][referencia]
...
...
...
Al final del documento:
[referencia]: url "etiqueta"
```

- Parámetros:
  - texto del recurso: texto del enlace.
  - referencia: marcador utilizado como referencia en el enlace.
  - url: dirección del recurso (absoluta o relativa).
  - "etiqueta": es opcional y muestra tooltip con información sobre el enlace.

### Ejemplo enlaces con referencia

```markdown
- [Enlace a Google][marcador1]
- [Karames Formacion][marcador2]
  ...
  ...
  ...
  Al final del documento:
  [marcador1]: https://www.google.es/ "Ir a Google"
  [marcador2]: https://formacion.karames.es/ "Ir a Plataforma de Formación"
```

- [Enlace a Google][urlgoogle]
- [Karames Formacion][urlkaramesformacion]

[urlgoogle]: https://www.google.es/ "Ir a Google"
[urlkaramesformacion]: https://formacion.karames.es/ "Ir a Plataforma de Formación"

## Enlaces automáticos

- Si sólo queremos mostrar la dirección del recurso, sin nada más.
- Poner la dirección entre los signos "<" y ">".

```markdown
- <https://www.google.es/>
- <https://formacion.karames.es>
```

- <https://www.google.es/>
- <https://formacion.karames.es>

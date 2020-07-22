# Enlaces e imágenes

En los documentos _Markdown_ podemos agregar enlaces a otros recursos, la manera es muy sencilla, solo se debe seguir la siguiente regla:

```markdown
[recurso](url etiqueta)
```

En esa regla la parte de **recurso** corresponde a los que mostrara el texto a la hora de ser interpretado, la **url** es la dirección del recurso, se pueden usar direcciones absolutas o relativas y finalmente la **etiqueta** es una cadena de texto opcional que nos dará información en un tooltip al poner el cursos sobre el enlace.

Ejemplo:

[Karames Formacion](https://formacion.karames.es/ "Ir a")

[Repositorio del curso](https://github.com/camaciasd/curso-markdown "Repositorio en GitHub del curso")

En código seria esto:

```markdown
[Repositorio del curso](https://github.com/camaciasd/curso-markdown "Repositorio en GitHub del curso")
```

La desventaja de esta regla para crear los enlaces es que a veces si se utiliza mucho un mismo enlace o si se tiene direcciones muy largas o complejas, esto puede dificultar la lectura del documento, por lo que _Markdown_ tiene la opción de crear enlaces con referencia, esto consiste en crear al final del texto una serie de etiquetas con la formula `[etiqueta]: url`, así después cuando quiera usarse ese enlace en alguna parte del documento se pondría de la forma `[recurso][etiqueta]`, eso facilita la lectura del código y se usa múltiples veces en mismo enlace nos evita el escribirlo varias veces.

Ejemplo:

[Enlace a Karames Formacion][urlkaramesformacion]

[Mi pefíl en Udemy][perfiludemy]

En código seria esto para el enlace:

```markdown
[Mi pefíl en Udemy][perfiludemy]
```

Y esto al final del documento:

```markdown
[perfiludemy]: https://www.udemy.com/user/carlos-antonio-macias-duarte/
```

Finalmente tenemos un tercer tipo de enlace, esto son los automáticos, son los mas simples, cuando lo que se quiere mostrar es directamente la dirección de un recurso sin poner algún texto que lo identifique, solo se pone la dirección entre signos de menor que y mayor que.

Ejemplo:

- <https://formacion.karames.es/>
- <https://github.com/camaciasd>

En código seria esto:

```markdown
<https://github.com/camaciasd>
```

Eso seria todo por la parte de enlaces, ahora sobre las imágenes se colocan de igual manera que la primera de poner enlaces, pero se le antepone el carácter \! al enlace, y en este caso el nombre del recurso es una cadena que mostrara si la imagen no esta disponible.

Ejemplo:

![Imagén que si existe](/img/markdown.png)
![Imagén que no existe](/img/Markdown0.png)

En código seria esto:

```markdown
![Imagén que si existe](/img/Markdown.png)
![Imagén que no existe](/img/Markdown0.png)
```

Mascota [^1] de Linux (Tux):

![[Tux]](/img/tux.png)
![Tux][logolinux]

- contenidos
- contenidos

  ![Tux enano](/img/tux_nano.png)

- continúa

[![alt text](/img/tux_nano.png)](http://wordpress.com/ "Title")
[![alt text][logolinux]](http://wordpress.com/ "Title")

[perfiludemy]: https://www.udemy.com/user/carlos-antonio-macias-duarte/
[urlkaramesformacion]: https://formacion.karames.es/ "probando"
[logolinux]: /img/tux.png

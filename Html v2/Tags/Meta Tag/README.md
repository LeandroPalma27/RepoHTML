# Meta tag

La etiqueta meta especifica los metadatos a utilizar en el documento HTML. Los metadatos son datos que describen a otros datos, asi de simple.

Estas etiquetas siempre van dentro de la etiqueta head, y no se muestran al final en la pagina web.

Por lo general se utilizan para especificar la juego de caracteres, descripcion de la pagina, palabras clave para un buen SEO, el autor del documento, compatibilidad con navegadores antiguos y la configuracion de la ventana grafica.

Ejemplo de uso de un meta para la parte grafica:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
```

Donde:

- El atributo name con el valor "viewport": Especifica instrucciones al navegador sobre como controlar las dimensiones y escala de la pagina web.
- El atributo content con el valor "width=device-width, initial-scale=1.0: Establece el ancho de la pagina para poder seguir el ancho de la pantalla del dispositivo (que variara dependiendo del dispositivo), y el "initial-scale=1.0", especifica el nivel de zoom con el que se cargara la pagina en el navegador.



### Meta charset

El meta charset permite especificar el juego de caracteres. Generalmente se usa UTF-8.

```html
<meta charset="UTF-8">
```

### Meta name

Este atributo en el meta, especifica el nombre del metadato en cuestion.

### Meta content

Este atributo especifica el valor que esta asociado al nombre del metadato descrito por la etiqueta name.


## Metas mas usados aparte de lo ya visto

Palabras clave (SEO):

```html
<meta name="keywords" content="Consolas, Spiderman, Videos, Superheroes, Musica, Araña, Spider, Valores">
```

Autor de una pagina:

```html
<meta name="author" content="Leandro Palma">
```

Actualizar cada cierto tiempo (en este caso cada 10 seg):

```html
<meta http-equiv="refresh" content="10">
```

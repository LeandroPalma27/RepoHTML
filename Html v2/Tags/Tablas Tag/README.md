## Tabla Tag

Las tablas, son elementos en el cual podemos organizar cualquier tipo de informacion. Es super importante aprender a usarlas en HTML. 

### Partes de una tabla:

- Table: Es la etiqueta padre de toda la tabla.

- Componentes principales de una tabla (thead, tbody y tfoot): Son respectivamente, la cabecera, el cuerpo y el pie de pagina de una tabla. 

- Filas en la tablas (tr): El elemento encargado de definir filas en una tabla es el tr, que vendria a ser los rows (filas) en la tabla. 

- Componentes de informacion (th (table head) y td (table data)): Son los elementos encargados de mostrar la informacion de la tabla en el DOM. El th es para la parte de la cabecera (visto desde un punto semantico) y el td es para la parte del cuerpo y el pie de pagina.

### Atributos HTML de una tabla mas usados (en cada elemento que la conforma): 

- Cellspacing: Define el espacio entre los bordes (es mejor usar border-spacing).

- Colspan: Define la cantidad de columnas que ocupara una celda o fila.

- Rowspan: Define la cantidad de filas que ocupara una celda o columna.

### Estilos de una tabla (nativo y bootstrap):

Importante:

En caso de querer una tabla con renglones de diferente color, como por ejemplo, las filas impares de color blanco y las pares de color gris, debemos usar la siguiente funcion de CSS.

```css
tr:nth-child(even) {
background-color: white;
}
```

La funcion recibe un parametro, donde si es even, se selecciona las filas pares, y si es odd, se selccionan las filas impares.


Bootstrap:

Realmente, no hace falta profundizar, ya que en la documentacion de bootstrap de explica a la perfeccion como realizar el uso correcto de sus tablas predefinidas.
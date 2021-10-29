## Elementos inline vs block

Un gran ejemplo de comparar estos dos tipos de elementos, es cuando se compara a un elemento div con un elemento span.

Los dos elementos no tienen un sentido logico al momento de estrucutrar las paginas web, solo se usan para separar partes de elementos con otras partes.

La unica diferencia, es que div es elemento de bloque, mientras que span es un elemento de linea.

Un elemento inline, ocupa un tamaño en relacion a su contenido. No puede modificarse su altura y/o ancho.

Un elemento block, ocupa todo un espacio en el DOM, por mas que su contenido no ocupe toda la pantalla. Se puede modificar su altura y/o ancho.

### ¿Y si queremos modificar el tamaño de un elemento inline?

Para eso, con CSS cambiamos la propiedad display del elemento, a inline-block.
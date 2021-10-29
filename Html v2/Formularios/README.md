# Formularios en HTML

Los formularios en html son algo muy importante de entender y manejar, ya que se suele usar informacion sensible en este tipo de tecnologias de validacion de informacion en la web.

Lo mas importante, es conocer los metodos http que se pueden usar en los formularios. Entre ellos solo hay dos, el metodo GET y POST.

## Ligar labels a elementos input

Con tan solo al atributo for del label, le colocamos el mismo identificador del input al cual queremos apuntar, ya habremos ligado y en caso de hacer click en el label, se dara foco a su input ligado.


## Atributo method

Si no se especifica, por defecto el metodo a usar es el GET.

### Get

Get es un metodo HTTP con el cual podemos procesar informacion para que el servidor pueda procesarla, valga la redundancia, y asi poder validar peticiones, etc.

Al usar get, el protocolo actua de una manera especifica, por ejemplo, en la URL se muestra un query string donde la informacion enviada a traves del formulario se puede visualizar. Se usa mas que todo para obtener informacion en funcion a algo en especifico.

VENTAJAS:

- La informacion puesta finalmente en la URL, se puede guardar como marcador para posibles consultas futuras, como mapas satelitales, busquedas en navegadores, etc.

- Si se retrocede, la informacion no se enviara.

DESVENTAJAS:

- La principal desventaja, es la vista simple de la informacion en la URL. A pesar de que se cifre, desde el usuario cliente puede verse de manera completa y sin cifrar.

- Otra desventaja seria que solo se permiten caraceres ASCII, por lo tanto, enviar informacion como datos binarios (audio, video, etc), no podria hacerse.

- La cantidad de caracteres es limitada en funcion al servidor (como mucho podrian ser 2048 caracteres).

- (Podria ser una desventaja o ventaja) La informacion de las url queda registrada como cadenas de texto.

### Post

Con post, lo que se hace es procesar la informacion para poder hacer algo con esa informacion ya validada. Por ejemplo, si validamos un login y queremos que se redirija a una pantalla de logeo exitoso, se puede usar POST.

### Get vs Post: ¿Que escoger para formularios?

Si bien es cierto, con get la informacion va en la URL, esta se termina cifrando, con lo cual es igual de seguro que post. Pero, la unica diferencia es que las peticiones GET se almacenan en un registro de peticiones como cadenas de texto, con lo cual ya no lo hace tan seguro para manejar informacion confidencial.

En todo caso, lo mejor es usa post, ya que la informacion confidencial es muy usada en la web y siempre es mejor prevenir que lamentar.

VENTAJAS:

- La principal ventaja, es que la informacion ya no se transimite a traves de la url, sino que va en el cuerpo de la peticion HTTP.

- La capacidad de enviar informacion es ilimitada (no se limita a solo 2048 caracteres ASCII).

DESVENTAJAS:

- La principal desventaja, es que cuando por alguna razon se retrocede el formulario que ya habia sido enviado con informacion, puede que se termine enviando dos veces la misma peticion, con lo cual en sistemas como ventas, podria ser muy peligroso.

¿Cuando usar get y cuando post?

Deberia ser simple de escoger: Get, cuando queremos modificar, personalizar, actualizar paginas web, hacer busquedas, donde no se maneje informacion confidencial y se pueda aprovechar la ventaja de poder guardar las url como marcadores.

Post, cuando se maneje informacion que sea confidencial, cuando se manejen datos como archivos y se hagan peticiones al servidor.

## Atributo action 

El atributo action especifica a donde apuntara el formulario (servidor) para poder enviar la informacion al servidor para que pueda ser procesada.

En caso de consumir una api, se usaria alguna libreria o la api fetch para poder validar esa informacion.

### Atributos mas usados en elementos que componen un formulario

- id (OBLIGATORIO)
- name (OBLIGATORIO)
- type (OBLIGATORIO)
- placeholder
- required

### Atributos mas usados en elemento form

- action
- method
- target
- autocomplete

## Elementos radiobuttons y checkbox 

Se usan para escoger opciones ya predefinidas en un formulario, los radio se usan para escoger una sola opcion a la vez, mietras que los check se usan para escoger multiples opciones.

### Radiobuttons

Son los clasicos puntitos que nos permiten seleccionar opciones, como las del genero, etc.

Para poder hacer que solo se pueda escoger una a la vez, se le da el mismo name a cada una de ellas.

### Checkbox

Son cajitas con check, permiten que se puedan selecionar varias opciones a pesar de estar relacionados.

### Conclusion:

Siempre lo mejor es que radiobuttons comom checkboxes deben estar relacionados con el mismo name, ya que es lo semanticamente correcto.

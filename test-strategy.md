## Prueba en el Desarrollo "Adivina tu número"

### Módulo de Pruebas Caja Negra

#### Diseño de la Página
##### Problema:
Se observa que el diseño de la página es muy simple. Como corrección, se deben realizar cambios necesarios, como agregar un submenú que describa en detalle las reglas del juego y un diseño que capture la atención del usuario.

#### Validación de Entrada
##### Problema:
Se valida en el sistema que el campo acepta números reales y no muestra un mensaje de error al accionar el botón.

##### Corrección:
Se corrigió la validación para garantizar que el campo acepte números reales sin mostrar mensajes de error al hacer clic en el botón.

##### Problema:
Se valida en el sistema que el campo acepta valores de tipo texto y no muestra un mensaje de error al accionar el botón.

##### Corrección:
Se corrigió la validación para garantizar que el campo acepte valores de tipo texto sin mostrar mensajes de error al hacer clic en el botón.

##### Problema:
Se observa que el sistema acepta valores iguales o menores a 0.

#### Análisis de Caja Blanca

##### Generación de Número Aleatorio
##### Problema:
El número que se genera aleatoriamente es incorrecto, ya que solo genera números de 0 a 10.

##### Corrección:
Se corrigió el código para generar números aleatorios entre 1 y 100, garantizando que estén dentro del rango especificado.

##### Número de Intentos
##### Problema:
Se detectó un error en la línea 46, que permitía solo 5 intentos al usuario en lugar de los 10 requeridos.

##### Corrección:
Se corrigió la línea 46 para permitir 10 intentos al usuario, cumpliendo con los requisitos del juego.

##### Evento addEventListener
##### Problema:
Se identificó un error en la escritura del nombre del evento `addEventListener`, lo que causaba un funcionamiento incorrecto.

##### Corrección:
Se corrigió el llamado al evento `addEventListener` para que se escriba correctamente y funcione según lo esperado.


##### Problema:
Se encontró un error en las líneas 65 y 70 del código fuente, que no reflejaban adecuadamente la lógica del juego.

##### Corrección:
Se corrigieron las líneas 65 y 70 para asegurarse de que:
- Si el valor ingresado por el usuario es mayor o menor que el número objetivo, se muestre el mensaje en color negro.
- Si el usuario supera los 10 intentos, se muestre el mensaje en color rojo.
- Si el usuario adivina el número, se muestre el mensaje en color verde.

##### Validación de Entrada
##### Problema:
Se detectó un error de funcionamiento en la línea 56, que representaba la funcionalidad para capturar el último número ingresado por el usuario.

##### Corrección:
Se corrigió la función para validar que el número ingresado esté dentro del rango de números enteros entre 1 y 100. Si el usuario ingresa un valor no válido, se muestra una alerta y no se registra como un intento.


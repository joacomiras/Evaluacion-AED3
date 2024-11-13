# Evaluacion AED3
Leer con atención el README, teniendo en cuenta la condición de entrega. De no cumplirse esto, la entrega será inválida y se evaluará con un  1 (uno).

# Metodología
Esta evaluación es un tanto particular como se darán cuenta. La misma consiste en realizar una librería para una pantalla LCD 20x4 (datasheet adjuntado en repositorio). Cada función que deban crear estará especificada tambien con su nombre, pero el tipo lo deberán determinar ustedes. 
Como último, deberán crear un código de ejemplo con la utilización de dicha librería donde se muestre el uso de alguna de sus funciones.
Una aclaración no menor es que no podrán utilizar nada por fuera de lo que brinda este repositorio. Cualquier otra búsqueda realizada o página abierta será de sanción y tendrá un 1(uno) en la evaluación. Quitando la posibilidad de poder rendir el recuperatorio.

# Consignas
Realizar una librería llamada *"LCD_I2C"* para la pantalla LCD 20x4 (2004A) con controlador I2C (HD44780U) que contenga las siguientes funciones:
* *LCD_Init()*: Inicializa la pantalla LCD. Donde se inicializará todo lo necesario para el correcto funcionamiento de la pantalla y la placa. Y, además, se encenderá la pantalla y se configurará el cursor.
* *LCD_Clear()*: Limpia la pantalla.
* *LCD_Print()*: Impime una cadena de texto en la pantalla.
* *LCD_SetCursor()*: Coloca el cursor en fila y columna deseada.
* *LCD_Command(uint8_t command)*: Enviará los comandos necesarios para el funcionamiento debido de la pantalla LCD. La escritura de dichos comandos será en dos partes, ya que el controlador trabaja en nibbles.
* *LCD_Write(uint8_t data)*: Por donde se enviarán datos hacia la pantalla.
* *LCD_ScrllDisplayRight()*: Funcion que hace desplazar la pantalla hacia la derecha.
* *LCD_ScrllDisplayLeft()*: Funcion que hace desplazar la pantalla hacia la izquierda.

# Método de entrega
Al finalizar la clase (a eso de las 17hs), se habilitará el uso de internet para la subida de la librería a un repositorio de GitHub. Dicho repositorio será subido a la tarea *"Evaluación 2° Cuatrimestre"* dentro de nuestro Classroom. Dentro del repositorio tienen que encontrarse tres archivos. Dos para la librería y uno del código de ejemplo. Se valorará la sintáxis y orden del código, como así también las partes aclaradas (comentarios).

# Aclaraciones finales
* Se prodrá usar la librería brindada en este repositorio para el protocolo I2C.
* Address de la pantalla LCD: *0x27*.
* Las filas no están numeradas del 0 al 3, sino que *0x80, 0xC0, 0x94, 0xD4* respectivamente.
* Utilizar *define* para todos los comandos, modos y/o pines utilizados, especificando en su nombre lo que hace y siempre en mayúscula.
* Cada función valdrá un punto. Los puntos restantes los darán la prolijidad y su habilidad para programar.
* Librería que esté completamente desordenada penalizará más de dos puntos, por lo que podría ser causante de desaprobación.

# README 
Trabajo Atelem Aplicación Andriod
Ampliación calculadora 

 ![image](https://github.com/Miquel121/README/assets/124579022/ebfe307d-27e2-4ff7-ab8a-f98db91a7257)




Miquel Ramos Serradell
Pablo Martinez Martinez
Grupo A4

La aplicación escogida para la realización del trabajo es la ampliación de la calculadora previamente creada en la practica 4. Para ello hemos añadido nuevas funcionalidades que implementan nuevas operaciones, para tener un abanico mas amplio respecto a la utilidad de nuestra aplicación. Para ello introduces un valor, escoges la operación que quieres realizar y introduces otro valor y se obtendrá el resultado de esa operación.
También hemos puesto a nuestro gusto la estética de la calculadora, cambiando la fuente, el logo y el color de nuestros botones.
Y lo configuramos tanto para mostrar la imagen horizontalmente como verticalmente.
 ![image](https://github.com/Miquel121/README/assets/124579022/a265c986-86e3-48d1-bbae-c4ccd5714619)
  ![image](https://github.com/Miquel121/README/assets/124579022/5022d95a-14e7-45ec-bd14-e4954fd7c11b)

 

 
Se presenta una descripción algorítmica de las clases e interfaces relacionadas, así como los aspectos más importantes y su interacción:

1.	Clase MainActivity: Esta clase extiende la clase AppCompatActivity y representa la actividad principal de la aplicación. Es responsable de gestionar la interfaz de usuario y las interacciones con los elementos de la calculadora. Algunos aspectos destacados de esta clase son:

•	Variables miembro:

OP_ANT: Una enumeración que representa la operación anterior pendiente de realizar.
estado: Una enumeración que representa el estado actual de la calculadora.
acumulador: Un double que actúa como el acumulador de operaciones.
operando2_str y operando2: Una cadena y un double que representan el segundo operando de las operaciones.
display: Un TextView que muestra los resultados y los operandos en pantalla.
df: Un objeto DecimalFormat utilizado para formatear la salida en pantalla.
Ans: Un double que almacena el resultado anterior.
•	Métodos:

onCreate(): Método que se llama cuando se crea la actividad. Aquí se realiza la inicialización de la calculadora, se enlaza el TextView y se configura el formato de salida.
alPulsarTecla(): Método que se ejecuta cuando se hace clic en un elemento de la interfaz. Utiliza una estructura switch para determinar la acción correspondiente según la tecla pulsada.
operar(): Método privado que realiza la operación matemática entre dos operandos según la operación especificada.
miStringToDouble() y miDoubleToString(): Métodos privados para convertir entre String y double.
onSaveInstanceState() y onRestoreInstanceState(): Métodos utilizados para guardar y restaurar el estado de la calculadora al cambiar la orientación de la pantalla, por ejemplo.
2.	Enumeración OPERACION: Esta enumeración define los diferentes tipos de operaciones matemáticas que se pueden realizar, como suma, resta, multiplicación, división, potencia, raíz, logaritmo y igual.

3.	Enumeración ESTADOS: Esta enumeración define los diferentes estados de la calculadora, como inicial, número y operación.

La clase MainActivity es la actividad principal de la aplicación y maneja la lógica de la calculadora. Utiliza enumeraciones para representar los tipos de operaciones y los estados de la calculadora. Los métodos y variables miembro permiten realizar cálculos, actualizar la interfaz de usuario y mantener el estado de la calculadora.
A la hora de realizar el trabajo hemos tenido un problema al realizar la ampliación lo hicimos ampliando el código que teníamos en la practica 4 y nos daban bien los resultados, luego a la hora de realizar el proyecto en el repositorio del trabajo nos daba un error en los switch (id) que no entendemos porque y no sabemos solucionar. Hemos comprobado que el código funcionaba según lo requerido pero no lo hemos sabido hacer funcionar en el directorito del trabajo. Siendo el siguiente error : C:\Users\PABLO\Desktop\TR_ATELEM\app\src\main\java\es\upv\etsit\gitst\trabajoatelem\MainActivity.java:163: error: constant expression required
                    case R.id.b_...

![java](http://alldonetechnology.com/wp-content/uploads/2017/06/java_banner1-e1498631671232.jpg)



## *¿ Que es java ?*


Java es un lenguaje de programación y una plataforma informática comercializada por primera vez en 1995 por Sun Microsystems. Hay muchas aplicaciones y sitios web que no funcionarán a menos que tenga Java instalado y cada día se crean más. Java es rápido, seguro y fiable. Desde portátiles hasta centros de datos, desde consolas para juegos hasta súper computadoras, desde teléfonos móviles hasta Internet, Java está en todas partes.


*El lenguaje Java se creó con cinco objetivos principales:*

Debería usar el paradigma de la programación orientada a objetos.
Debería permitir la ejecución de un mismo programa en múltiples sistemas operativos.
Debería incluir por defecto soporte para trabajo en red.
Debería diseñarse para ejecutar código en sistemas remotos de forma segura.
Debería ser fácil de usar y tomar lo mejor de otros lenguajes orientados a objetos, como C++.

![java](http://www.capitani.com.br/wp-content/uploads/2017/07/java-banner.jpg)

## *¿Para qué sirve Java?*
Java sirve para crear aplicaciones y procesos en una gran diversidad de dispositivos. Se base en programación orientada a objetivos, permite ejecutar un mismo programa en diversos sistemas operativos y ejecutar el código en sistemas remotos de manera segura.

Su ámbito de aplicación es tan amplio que Java se utiliza tanto en móviles como en electrodomésticos. Muchos programadores también utilizan este lenguaje para crear pequeñas aplicaciones que se insertan en el código HTML de una página para que pueda ser ejecutada desde un navegador.





*Características del lenguaje Java*
Dentro de las características del lenguaje Java encontramos:

# Independiente de Plataforma
Cuando compilamos código fuente Java no se genera código máquina específico, si no que se generan bytecodes, los cuales son interpretados por la Java Virtual Machine (JVM), posibilitando que un mismo código fuente pueda ser ejecutado en múltiples plataformas.

# Orientado a Objetos
Cualquier elemento del lenguaje Java es un objeto. Dentro de los objetos se encapsulan los datos, los cuales son accedidos mediante métodos.

# Sencillo
Java está enfocado para ser un lenguaje fácil de aprender. Simplemente se deberán de entender los conceptos básicos de la programación orientada a objetos (POO).

# Seguro
Es seguro ya que los programas se ejecutan dentro de la Java Virtual Machine (JVM) en un formato de “caja de arena”, de tal manera que no pueden acceder a nada que esté fuera de ella.

Tiene una validación sobre los bytecodes para comprobar que no hay códigos de fragmento ilegal.

# Arquitectura Neutral
Independientemente de que se ejecute en una arquitectura de 32bits o de 64bits. En Java los tipos de datos siempre ocupan lo mismo.

# Portable
Java no tiene nada que dependa de la plataforma, lo cual le hace que sea portable a diferentes plataformas.

# Robusto
El lenguaje Java intenta controlar las situaciones de error en los procesos de compilación y de ejecución, reduciendo de esta manera el riesgo de fallo.

Además Java realiza el control total de la memoria alocándola y retirandola mediante un garbage colletor, de tal manera que no podemos utilizar punteros para acceder a ella.

# Multi-hilo
Java nos permite la programación concurrente, de tal manera que un único programa puede abrir diferentes hilos de ejecución.

# Interpretado
Los bytecodes son interpretados en tiempo real a código máquina.

# Alto Rendimiento
Java ofrece compiladores Just-In-Time que permiten tener un alto rendimiento.

# Distribuido
El lenguaje Java está pensando para ser ejecutado en arquitecturas distribuidas, como pueda ser Internet.



*Instalacion de java en linux*

[Descargar java](https://www.java.com/es/download/help/linux_install.xml "Explicacion de como descargar en linux en su pagina oficial")

Para instalar el runtime y el kit de desarrollo de Java, teclea en la terminal:

sudo apt install openjdk-8-jdk openjdk-8-jre



## *MINI TUTORIAL*

## Declaración de variables locales

Las variables locales se declaran igual que los atributos de la clase:
Tipo NombreVariable [= Valor];
Ej: int suma;
float precio;
Contador laCuenta;
Sólo que aquí no se declaran private, public, etc., sino que las variables definidas dentro del método sólo son
accesibles por él.
Las variables pueden inicializarse al crearse:
Ej: int suma = 0;
float precio = 12.3;
Contador laCuenta = new Contador ( );



## Asignaciones a variables

Se asigna un valor a una variable mediante el signo =:
Variable = Constante | Expresión ;
Ej: suma = suma + 1;
precio = 1.05 * precio;
laCuenta.cnt = 0;
El último caso es válido si cnt es una variable pública de la clase Contador. Personalmente no creo
conveniente acceder directamente a variables de otro objeto, ya que futuras modificaciones del objeto llamado
o del que llama puede propender la difusión de errores… Es mejor usar métodos como getCuenta o un
hipotético inicializarContador para ello. De hecho, algunos sugieren que todas las variables de una clase se
declaren como private .
En el primer caso, o sea en general:
Variable = Variable Operador Expresión;
se puede escribir en forma más sencilla:
Variable Operador= Expresión;
Por ejemplo, suma = suma + 9 - cantidad;
puede escribirse: suma += 9-cantidad;
y precio = precio * 0.97;
como: precio *= 0.97;




## Operaciones matemáticas


![java](https://tutorias.co/wp-content/uploads/2013/04/serieMatematicaPIJava.jpg)

Hay varios tipos de operadores:
Unarios: + - ++ -- ~ ! (tipo) …..etc.
Se colocan antes (o en algunos casos después) de la constante o expresión.
Por ejemplo: -cnt; // cambia de signo; por ejemplo si cnt es 12 el resultado es -12; cnt no cambia.
++cnt; // equivale a cnt += 1;
cnt++; // equivale a cnt +=1; veremos la diferencia al hablar de estructuras de control
--cnt; // equivale a cnt -= 1;
cnt--; // equivale a cnt -= 1;
Binarios: + - * / % …..etc.
Van entre dos constantes o expresiones o combinación de ambas.
Por ejemplo: cnt + 2; // debuelve la suma de ambos.
promedio + ( valor / 2); // como se ve, se pueden usar paréntesis.
horas / hombres; // división.
acumulado % 3; // resto de la división entera entre ambos.
Nota: + sirve también para concatenar cadenas de caracteres; hablaremos de String y StringBuffer pronto.
Cuando se mezclan Strings y valores numéricos, éstos se convierten automáticamente a cadenas:
"La frase tiene " + cant + " letras"
se convierte en: "La frase tiene 17 letras" // suponiendo que cant = 17



## Las estructuras de control

Las estructuras de control en Java son básicamente las misma que en C, con excepción del goto, que no existe
(al fin un lenguaje serio! )


![java](http://www.kilobolt.com/uploads/1/2/5/7/12571940/5192811_orig.png)


if…[else]
La más común de todas, permite ejecutar una instrucción (o secuencia de instrucciones) si se da una condición
dada (o, mediante la cláusula else, ejecutar otra secuencia en caso contrario).
if (expresión_booleana) instrucción_si_true;
[else instrucción_si_false;]
o bien:
               if (expresión_booleana) {
instrucciones_si_true;
}
else {
instrucciones_si_false;
}
Por ejemplo:
public final String toString() {
if (y<0)
return x+"-i"+(-y);
else
return +x+"+i"+y;




## While

Permite ejecutar un grupo de instrucciones mientras se cumpla una condición dada:
while (expresión_booleana) {
instrucciones…

}
Por ejemplo:
while ( linea != null) {
linea = archivo.LeerLinea();
System.out.println(linea);
}

## Do…while

Similar al anterior, sólo que la condición se evalúa al final del ciclo y no al principio:
do {
instrucciones…
} while (expresión_booleana);
Por ejemplo:
do {
linea = archivo.LeerLinea();
if (linea != null) System.out.println(linea);
} while (linea != null);


## For
También para ejecutar en forma repetida una serie de instrucciones; es un poco más complejo:
for ( instrucciones_iniciales; condición_booleana; instruccion_repetitiva_x ) {
instrucciones…
}
Si bien las instrucciones pueden ser cualquiera (el bucle se repite mientras la condición sea verdadera), lo
usual es utilizarlo para "contar" la cantidad de veces que se repiten las instrucciones; se podría indicar así:
for ( contador = valor_inicial; contador < valor_final; contador++ ) {
instrucciones…
}
Por ejemplo:
for ( i=0; i<10; i++ ) {
System.out.println( i );
}
o, para contar hacia atrás:
for ( i=10; I>0; I-- ) {
System.out.println( i );
}


## EL ZEN DE JAVA

explicit.compareTo (implícito) == 

- Por ejemplo, uno no simplemente envía una pequeña letra de texto, sino que un MimeMessage creado para una sesión configurada con Propiedades se envía a través de un SMTPTransport utilizando PasswordAuthentication.

- Marcos sobre bibliotecas. ¿Recuerdas la última vez que un entrevistador te preguntó con qué bibliotecas has trabajado? Yo tampoco.

- Los sistemas de compilación deben ser crípticos, y preferiblemente de palabras. Las secuencias de comandos de compilación no deben, bajo ninguna circunstancia, verse como lo hacen y aún deben tomar varias pantallas para las tareas más simples.

- Si la implementación es difícil de explicar, es un patrón de diseño establecido.

- Un equipo es más importante que un hacker individual. Porque un equipo puede hacer cosas hermosas como ERP, CRM, integraciones complejas y un hacker no puede. Y no lo haría.

- Las construcciones del lenguaje que explican los efectos secundarios están mal vistas (excepciones marcadas). Morir en medio del flujo de control es recibido (lanzando explícitamente excepciones de tiempo de ejecución, llamando a los métodos en nulo).

- Un error de mil millones de dólares es demasiado barato para ser abordado.

- Nunca salgas del arenero.

- El uso de herramientas no creadas específicamente para Java está prohibido. Idealmente, las herramientas también deberían estar escritas en Java.

- Puede ser excluido (durante las revisiones de código, p. Ej.) Por usar demasiadas interfaces, no usar suficientes interfaces, usar demasiados / métodos cortos, crear pocos métodos enormes, crear abstracciones innecesarias, incluir demasiadas responsabilidades en una abstracción, usar OOP enrevesada, ser demasiado procesal, etc.

- Se sorprenderá de lo lejos que puede llegar antes de comenzar a trabajar con el código compatible con OO que hace lo que necesita. Muy, muy lejos ...

- La complejidad accidental es indistinguible de la complejidad inherente.

- Si algunas de sus clases no tienen estado, o no combinan el comportamiento con él, o no mutan ese estado con ese comportamiento, entonces ¿por qué usar Java?
 
-  un campo sin un par getter / setter es una pérdida de espacio.

- Los sistemas escritos en Java deben consistir en controladores, controladores, administradores, servicios, componentes, ayudantes, utilidades, convertidores, fábricas, servidores proxy, agrupaciones (y combinaciones de esos) que operan datos, informaciones, artículos, nodos, modelos, contenedores, contenedores (y combinaciones) y colecciones de esos.

- Nirvana es donde todos los métodos tienen cero argumentos porque se inyectan todas las dependencias. Como todavía no está allí, la clase crítica para su tarea actual tiene 6 métodos sobrecargados con 8 a 15 argumentos.

- Pasar con éxito una entrevista de diseño de sistemas y responder todas las preguntas relacionadas con patrones le da la oportunidad de trabajar en otra base de código de mierda.

- Los amigos no permiten que los amigos se desarrollen en Java sin un IDE. Es imposible de todos modos.

- Cuando se enfrente a un código ilegible / no mantenible, culpe al lenguaje y proponga usar el sustituto actual de moda. El mejor de los casos: nadie aprueba reescribir el sistema, usted sigue pensando en usted como un genio no apreciado. El peor de los casos: está aprobado y se emplean décadas para obtener un sistema DOA escrito en un idioma en el que ya nadie esté interesado.


Creo que, desde el punto de vista práctico, Java sigue siendo uno de los mejores lenguajes, si no el mejor. Cada vez que elijo lógicamente un lenguaje de programación para el backend, casi siempre lo uso. Es solo que ... siento mucha nostalgia por los momentos en que programé en Perl, con la sensación de que todo es posible y que eres parte de una comunidad, con toda su magia y concisión y sin redes de seguridad. Esos fueron los días.

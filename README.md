# Programación Orientada a Objetos - UNAL

## Clase 5: Clases y Objetos

### Clase
Una clase es un *plano* o *plantilla* para crear objetos. Define un tipo de objeto especificando los datos que puede contener y los métodos (comportamientos) aplicables. 

**Ejemplos:**
 - Clase Fruta podría definir atributos como color y sabor, y métodos como madurar().
 - Clase de Vehículos como un concepto general. Todos los vehículos comparten características comunes como tener medios de locomoción y la capacidad de transportar personas o cosas, pero cada tipo (coche, bicicleta, avión) tiene sus propias especificaciones.

<br>
 <div align="center">
    <img src="./assets/Clases.png" alt="Diagrama clases" width="700" height="auto">
</div>


### Modelado por Clases
El modelado por clases permite a los desarrolladores organizar y estructurar su software de manera que refleje más fielmente el mundo real. En general facilita la comprensión del sistema al modelar entidades del mundo real de manera intuitiva. 

### Objeto
Un objeto es una *instancia* de una clase. Posee los atributos definidos por su clase y es capaz de realizar los comportamientos (métodos) definidos por ella. 

**Ejemplos:**
- Una instancia de la clase Fruta podría ser una manzana específica, con un color rojo y un sabor dulce.
- Una instancia de vehículo puede ser un Automóvil, con color rojo, locomoción por motor de combustión, y comportamientos de encender, frenar y apagar.

<br>
 <div align="center">
    <img src="./assets/Objetos.png" alt="Diagrama clases" width="700" height="auto">
</div>

## Diseño Orientado a Objetos (OOP)
El **OOP** es una metodología de diseño y programación que se centra en el uso de objetos y clases. Su función principal es modelar datos, tratando de extraer sus atributos y comportamientos. Su enfoque primario es centrarse en objetos que representan conceptos del mundo real 

### Abstracción
La abstracción es un principio fundamental del OOP que implica enfocarse en las características esenciales de un objeto, ignorando las menos importantes o irrelevantes. 

### Abstracción en el Mundo Real
Los seres humanos abstraen constantemente, simplificando complejidades para entender y interactuar con el mundo. Por ejemplo, al considerar un automóvil, nos enfocamos en su funcionalidad (conducir, frenar, acelerar) más que en los detalles complejos de su funcionamiento interno.

Al usar un televisor, interactúas con un conjunto limitado de controles (botones para cambiar el canal, ajustar el volumen, etc.), sin necesidad de entender la complejidad interna de cómo funciona el televisor.

## Datos, Atributos y Comportamientos
- **Datos** describen los estados de un objeto.
- **Atributos** son características específicas de un objeto.
- **Comportamientos** son las acciones que un objeto puede realizar.

<br>
 <div align="center">
    <img src="./assets/instancias.png" alt="Diagrama clases" width="700" height="auto">
</div>

## Herencia y Composición
La Herencia permite que una clase herede atributos y métodos de otra clase, facilitando la reutilización de código y la creación de jerarquías de clases.

Composición implica construir clases complejas a partir de la inclusión de objetos de otras clases, promoviendo una fuerte separación y modularidad.

### Comparación entre Herencia y Composición
Mientras que la herencia establece una relación `es un/a` (por ejemplo, un Perro es un Animal), la composición establece una relación `tiene un/a` (por ejemplo, un Coche tiene un Motor). La composición es generalmente preferida para mantener una baja acoplamiento y una alta cohesión.

**Ejemplos de Herencia:**

 - Un pato es un tipo de ave, por lo que hereda características comunes de las aves, como tener plumas y la capacidad de volar (aunque no todas las aves vuelan).
 - Una clase Pato puede heredar de una clase Ave, obteniendo sus métodos y atributos, y también puede tener sus propios métodos, como nadar().

**Ejemplos de Composición:**

 - Un coche tiene un motor. En lugar de ser un tipo de motor, el coche compone un motor entre sus partes.
 - La clase Coche puede contener un objeto Motor como atributo, lo que le permite acceder a los métodos del motor, como arrancar_motor().

## UML (Lenguaje Unificado de Modelado)
UML es una herramienta estándar para especificar, visualizar, construir y documentar los artefactos de sistemas de software. Facilita la representación gráfica de clases, objetos, y sus relaciones, a través de diversos diagramas, como los diagramas de clases y de secuencia.

### Caso de Estudio: Sistema de Biblioteca
Imagina un sistema de biblioteca donde Libro es una clase con atributos como titulo y autor, y métodos como prestar() y devolver(). Una clase Usuario podría tener atributos como nombre y id, y métodos para registrar() y buscarLibros(). Utilizando composición, la biblioteca podría incluir objetos de tipo Libro y Usuario, gestionando las interacciones entre ellos.
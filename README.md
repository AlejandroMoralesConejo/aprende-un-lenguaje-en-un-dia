# Aprende un lenguaje de programación en un día (ejercicio voluntario para subir nota).

## Introducción

Cuando te sacaste el carnet de conducir, aprendiste las normas de circulación así como los fundamentos básicos para manejar un coche: volante, marchas, freno, acelerador, embrague, retrovisores... Seguramente, el coche que conduces ahora es diferente al que utilizaste para aprender a conducir, no obstante, lo puedes llevar sin problema. Cada coche tiene sus peculiaridades, pero quien sabe manejar un automóvil, puede adaptarse a las medidas, tacto y comportamiento de un vehículo en cuestión de horas.

Aprender a programar es como aprender a conducir. Si tienes una base sólida de programación y sabes manejar con soltura los tipos de datos, bucles, arrays, clases, métodos, etc. podrás pasar de un lenguaje a otro en un período relativamente corto, simplemente tendrás que adaptarte a la sintaxis y a las peculiaridades del nuevo lenguaje.

Con este ejercicio se pretende despertar el interés por otros lenguajes de programación distintos al que el alumno está estudiando como primer lenguaje.

Sigue los pasos que se indican a continuación.

## Creación del equipo

Este ejercicio se debe hacer en grupos de 3 alumnos. Uno de ellos será el representante del grupo.

## Forkea forkea

El representante del grupo debe hacer un *fork* de este repositorio para utilizarlo como base.

## Añadiendo colaboradores

El encargado del grupo deberá añadir como colaboradores del repositorio *forkeado* a los otros dos miembros, para trabajar todos sobre los mismos archivos. Cuando alguien es colaborador en un repositorio, puede hacer *push* a él sin necesidad de pedir permiso o hacer *pull request*.

Para añadir colaboradores hay que hacer click en la pestaña *Settings* y seleccionar luego *Collaborators* en el menú.

## Miembros del grupo

Escribe aquí los miembros del grupo. El primero es el representante o encargado.

* Alejandro Morales Conejo
* Cristian Lobo Marrozos
* Javier Molina Maqueda

## Lenguaje de programación

El profesor llevará una cajita llena de papelitos con los nombres de distintos lenguajes de programación. Los encargados de cada grupo meterán la mano en la caja y sacarán dos papelitos, de los cuales el grupo elegirá uno. No se permite hacer intercambio de papelitos entre grupos.

Escribe el lenguaje de programación elegido por el grupo.

* C++

Los papelitos se han recortado de este [documento](lenguajes_de_programacion.pdf).

## Información sobre el lenguaje

¿Qué es?

C++ es un lenguaje de programación diseñado en 1979 por Bjarne Stroustrup. La intención de su creación fue extender al lenguaje de programación Cmecanismos que permiten la manipulación de objetos. En ese sentido, desde el punto de vista de los lenguajes orientados a objetos, el C++ es un lenguaje híbrido.

<img src="https://aprendiendoarduino.files.wordpress.com/2014/11/2afd4-cpp.jpg?w=396&h=396">

¿Por qué se llama así?

En programación, muchos lenguajes utilizan el operador ++ para incrementar el valor de una variable. De esta manera se puede decir que C++ es la continuación del lenguaje C.

Características:

-	Sintaxis heredada de C.
-	Tiene un estándar ISO.
-	Lenguaje fuertemente tipado.
-	Sobrecarga de operadores
-	Soporta expresiones Lambda, también llamadas funciones anónimas.
-	Control de excepciones.
-	Biblioteca estándar (plantillas de clases, soporte multihilo)
-	Compatibilidad con C.
-	Uso de punteros
-	Tiene un gran número de compiladores en diferentes plataformas y sistemas operativos.
-	Eficiencia con el hardware.

Una de sus principales desventajas es su complejidad.


## Herramientas de desarrollo
Necesitaremos un IDE (Entorno de Desarrollo Integrado) para escribir y compilar el código.
El más popular es Visual Studio Code que es libre y gratuito.
Además, hay otras opciones como Netbeans, Eclipse, Dev C++ o Code::Blocks que es muy popular entre gente que empieza a programar al requerir menos recursos.
<img src="https://i1.wp.com/justcode.me/wp-content/uploads/2017/08/Top-30-Best-IDEs-and-Compilers-for-C.jpg?resize=686%2C474">

Por otro lado, hay compiladores online, cómodos para probar el lenguaje como en este caso. Elegiremos este: https://www.onlinegdb.com/online_c++_compiler

## Poniendo en práctica el lenguaje

Pon en práctica el lenguaje de programación realizando los siguientes ejercicios. Para cada uno de los ejercicios, pega el código fuente de la solución y una captura de pantalla.

### 1. ¡Hola mundo!

Realiza un programa que muestre por pantalla la frase **¡Hola mundo!**.
```C++
#include <iostream>

using namespace std;

int main()
{
    cout<<"¡Hola Mundo!";

    return 0;
}
```

### 2. Pirámide

Dada una altura introducida por el usuario, realiza un programa que pinte una pirámide a base de asteriscos con la altura indicada.
```C++
#include <string>
#include <iostream>

using namespace std;

int main()
{
    int altura;
    string relleno = "*";
    int espacios;
    int planta = 1;
    int longitudLinea = 1;
    
    cout<<"Por favor, introduzca la altura de la pirámide: ";
    cin>>altura;
    
    espacios = altura-1;

    while(planta <= altura){
        //insertar espacios
        for(int i=0; i<espacios; i++){
            cout<<" ";
        }
        
        //pintar la linea
        for(int i=0; i<longitudLinea; i++){
            cout<<relleno;
        }
        cout<<"\n";
        
        planta++;
        espacios--;
        longitudLinea = longitudLinea + 2;
        
    }

    return 0;
}

```

### 3. Arrays y números aleatorios

Realiza un programa que rellene un array (o una estructura similar) con 20 números enteros aleatorios entre 1 y 100 y que seguidamente los muestre por pantalla. A continuación, se deben pasar los números primos a las primeras posiciones del array y los no primos a las posiciones restantes. Muestra finalmente el array resultado.

## Presentación de resultados

Cada equipo explicará al resto de la clase lo aprendido durante la realización del ejercicio. Todos los miembros de cada equipo deben participar en la explicación. Se puede utilizar como material de base para la presentación el repositorio de GitHub.

## Recompensa

* Todos los alumnos que realicen correctamente la actividad tendrán 0'25 puntos extra en la nota del trimestre.

* Los miembros del equipo más votado ganarán un premio.

:star: Si te ha gustado este ejercicio, dale una estrellita al [repositorio original](https://github.com/LuisJoseSanchez/aprende-un-lenguaje-en-un-dia).


# APUNTES JAVA

Compilar archivo .java --> **javac _"nombredelarchivo.java"_** (con extensión)

Ejecutar archivo compilado --> **java _"nombredelarchivo"_** (sin extensión)

### BLUEJ

Cuando abrimos un proyecto por primera vez con BlueJ, este creara un nuevo archivo con la extensión **.bluej**. Este archivo contiene información sobre la fecha de creación del programa. Al abrir el archivo .bluej, se abrirá el programa BlueJ con el proyecto en concreto.

Con la opción **_"Abrir no BlueJ"_** podemos abrir paquetes existentes creados sin BlueJ. Con **_"Abrir proyecto"_** solo podremos abrir paquetes creados con BlueJ.

[Captura 2](https://i.imgur.com/6NFg2SG.png) --> Antes de abrir el proyecto en BlueJ

[Captura 3](https://i.imgur.com/s3cUU1N.png) --> Después de abrir el proyecto en BlueJ

### INVOCANDO MÉTODOS

[Captura 1](https://i.imgur.com/M4FbZAn.png)

[Captura 2](https://i.imgur.com/Fn13v8c.png)

[Captura 3](https://i.imgur.com/SIKiUD8.png)

### INSPECTOR DE OBJETOS

[Uso del inspector de objetos](https://i.imgur.com/57lDz7T.png)

[Uso del inspector de objetos de nuevo](https://i.imgur.com/RP0fcIb.png)

### INVOCANDO METODOS PARA CREAR UN DIBUJO

[Imagen de la casa y el sol creada con BlueJ](https://i.imgur.com/s9WJMFc.png)

Estado de un objeto: conjunto de valores de los atributos del objeto en un momento dado.

**PARED:**

square1 = new Square()

square1.makeVisible()

square1.moveHorizontal(-100)

square1.changesize(80)

**VENTANA:**

square2 = new Square()

square2.makeVisible()

square2.changeColor("black")

square2.changeSize(30)

square2.moveHorizontal(-90)

square2.moveVertical(15)

**TEJADO:**

triangle1 = new Triangle()

triangle1.makeVisible()

triangle1.changeSize(40,120)

triangle1.moveHorizontal(140)

triangle1.moveVertical(-55)

**SOL:**

circle1 = new Circle()

circle1.makeVisible()

circle1.changeColor("yellow")

circle1.changeSize(50)

circle1.moveHorizontal(80)

circle1.moveVertical(-30)

### ESCRIBIENDO CODIGO JAVA EN EL CODE PAD

[Primer uso del Code Pad](https://i.imgur.com/OZ4xaqd.png)

### ESTUDIANDO EL CODIGO FUENTE

[Estudio de bloque de código](https://i.imgur.com/BFzHvq9.png)

### CAMBIANDO EL MÉTODO DRAW POR PRIMERA VEZ

[Captura 1. Listado de commits](https://i.imgur.com/w3GAFbd.png)

[Captura 2. Último commit](https://i.imgur.com/PrujpZv.png)

[Captura 3. Cambios del último commit](https://i.imgur.com/cLbOXEB.png)

Lo que más me ha costado ha sido asignar los atributos para que los objetos, como el sol, se situen en la posición exacta.

### ANIMANDO LA PUESTA DE SOL

[Captura 1. Listado de commits](https://i.imgur.com/b48Owry.png)

[Captura 2. Último commit](https://i.imgur.com/2Sxs1Bm.png)

[Captura 3. Cambios del último commit](https://i.imgur.com/HmUlgWv.png)

Lo que me costó fue ajustar el número de pixeles justos que el sol tenía que moverse hacia abajo.

### ANIMANDO LA ENTRADA EN ESCENA DE UNA PERSONA

[Captura 1. Listado de commits](https://i.imgur.com/3ynyLwX.png)

[Captura 2. Último commit](https://i.imgur.com/p3Kaa0I.png)

[Captura 3. Cambios del último commit](https://i.imgur.com/2zvAIAd.png)

Al principio no habia creado a la persona en el metodo atardecer, por lo que no funcionaba correctamente y se mostraba un error.

### CREANDO LA BASE DE DATOS DE ALUMNOS DE LA CLASE

[Alumnos de mi propia clase](https://i.imgur.com/2lHvpXN.png)

### ENTENDIENDO COMO LOS OBJETOS SE INDICAN COMO PARÁMETROS

[Detalles en la clase actual en la que estás](https://i.imgur.com/Qi3pRJD.png)

[Parámetro del metodo _matricularAlumno_](https://i.imgur.com/cTJNGd8.png)

[Parámetros del metodo _setTutor_](https://i.imgur.com/ueIC0lS.png)

[Zona de declaración de atributos](https://i.imgur.com/deNSYuZ.png)

### DETECTANDO PALABRAS RESERVADAS

[Palabras reservadas existentes en la clase _maquina-expendedora-simple_](https://i.imgur.com/ooBRk1M.png)

### ENTENDIENDO LA ESTRUCTURA DE UNA CLASE

[Estructura de la clase _maquina-expendedora-simple_](https://i.imgur.com/2JSQav0.png)

#### Atributos:

- precioBillete

- balanceClienteActual

- totalDineroAcumulado

- estacionOrigen

- estacionDestino

#### Constructor:

- MaquinaExpendedoraSimple(int precioDelBillete, String origen, String destino)

#### Métodos:

- getPrecioBillete

- getBalanceClienteActual

- introducirDinero

- imprimirBillete

### ESTUDIANDO LA CABECERA DE LOS CONSTRUCTORES

[Código fuente de la clase](https://i.imgur.com/KgCHVia.png)

### ESTUDIANDO LA INICIALIZACIÓN DE LOS ATRIBUTOS

[Código fuente original del constructor](https://i.imgur.com/d6v0npy.png)

[Código fuente modificado del constructor](https://i.imgur.com/wdG8Uxm.png)

- En la captura 1, todos los atributos se estaban inicializado explícitamente.

- En la captura 2, los atributos que se inicializaban explícitamente eran **balanceClienteActual** y **estaciónDestino**; y los que se inicializaban implícitamente eran todos los demás (**precioBillete**, **totalDineroAcumulado** y **estacionOrigen**)

- Los valores de **precioBillete** y **totalDineroAcumulado** son 0, mientras que el valor de **estacionOrigen** es nulo.

### ESTUDIANDO EL ÁMBITO Y TIEMPO DE VIDA

[Ámbito del atributo precioBillete y del parámetro precioDelBillete](https://i.imgur.com/g2bEzU5.png)

- El tiempo de vida del parametro **precioDelBillete** permanece hasta que se ejecuta el constructor.

- El tiempo de vida del atributo **precioBillete** coincide con el tiempo de vida del objeto (en este caso, la máquina expendedora).

### ESTUDIANDO LAS ASIGNACIONES

[Instrucciones de asignación en la clase maquina-expendedora-simple](https://i.imgur.com/Pyo5Q1T.png)

### ESTUDIANDO LOS METODOS DE LA CLASE MÁQUINA EXPENDEDORA SIMPLE

[Estudio de los métodos de la clase maquina-expendedora-simple](https://i.imgur.com/k8OTKPp.png)

### DISTINGUIENDO LOS USOS DEL OPERADOR DE CONCATENACIÓN

[Usos del operador + en el método imprimirBillete de la clase maquina-expendedora-simple](https://i.imgur.com/nfnFIzY.png)

- Las concatenaciones de cadenas contienen siempre valores de tipo **string**, mientras que las operaciones de suma contienen valores de tipo **int**.

### Pensando una instrucción condicional en pseudocódigo
~~~
if (es Lunes) {
    no tengo clase las dos ultimas horas y salgo antes de clase;  
}
else {
  tengo todas las horas y salgo a la hora normal;   
}
~~~

Un **pseudocódigo** es una manera de definir los algoritmos, es decir, los pasos necesarios para resolver un problema. Es un paso intermedio entre los diagramas de flujo y los lenguajes de programación.

### Investigando sobre los operadores relacionales

| Operando 1 | Operador | Operador 2 | Significado |
| -- | -- | -- | -- |
| a | < | b | menor que |
| a | > | b | mayor que |
| a | <= | b | menor o igual que |
| a | >= | b | mayor o igual que |
| a | == | b | igual que |
| a | != | b | distinto que |

### Escribiendo una instrucción condicional en pseudocódigo

~~~
if (a + b == ab * ab - 740) {
    invitar a otra copa;
}
else {
    invitar a unos chupitos;
}
~~~

### Estudiando la instrucción condicional de introducirDinero

- Para ejecutar el camino **if** en _introducirDinero_ debemos introducir una cantidad superior a 0 (sin incluir). Si no salta mensaje de error y se actualiza el balance actual, significa que ha seguido este camino correctamente.

- Para ejecutar el camino **else**, debemos introducir una cantidad igual o inferior a 0 (negativa). Si salta un mensaje de error, significa que ha seguido este camino.

- Si el valor introducido es 0, salta el mismo error que si el número fuera negativo, ya que el valor debe ser superior y **SIN INCLUIR** el número 0.

### Investigando la nueva versión del método imprimirBillete

[Diferencias entre el método imprimirBillete de la máquina mejorada con respecto a la simple si se imprime el billete](https://i.imgur.com/dW5EdiB.png)

### Comprobando las instrucciones condicionales sin parte else

- Si la cantidad de dinero introducida es valida y suficiente para pagar el billete, se ejecuta el código normal. En cambio si dicha cantidad no es suficiente para pagar el billete, no ocurre nada porque no hay parte **else** en el código.

[Método imprimiBillete sin parte else](https://i.imgur.com/yWH9ysa.png)

### Investigando cómo escribir la instrucción condicional

**- Un camino:**
~~~
if (hace frio) {
    me pongo una chaqueta;  
}
~~~

**- Dos caminos:**
~~~
if (hace frio) {
    me pongo una chaqueta;  
}
else {
    voy con manga corta;
}
~~~

**- Tres caminos:**
~~~
if (esta nevando) {
    me pongo un abrigo;  
}
else if (hace frio) {
    me pongo solo una chaqueta;
}
else {
    voy en manga corta; 
}
~~~

### Escribiendo otra instrucción condicional en pseudocódigo

~~~
if (a >= 65) {
    regalo de una copa y una botella de cava;  
}
else if (a >= 18) {
    regalo de una copa;
}
else {
    no está permitida la entrada; 
}
~~~

### Entendiendo el indentado de código

[Ámbitos en la clase MaquinaExpendedoraMejorada](https://i.imgur.com/YKX5Evl.png)

- **Indentar el código** es hacer espacios hacia la derecha para mover una linea de código, ya sea con la tecla espacio o con tabulación.

**Método mal indentado:**
~~~
/**
     * Devuelve el precio del billete
     */
    public int getPrecioBillete() {
    return precioBillete;
    }

    /**
     * Devuelve la cantidad de dinero que el cliente actual lleva introducida
     */
    public int getBalanceClienteActual() {
    return balanceClienteActual;
    }
~~~

### Practicando el indentado de código
~~~
void temperaturaMaximaMensual(int array[]) {
    int tmp=0;
    String cad="";
    int array2[] = new int[MAX];
         
    for(int i=0;i<array.length;i++) {
        array2[i]=array[i];
    }
     
    int k=0,x=0,c=0;
    for(int i=1;i<array2.length;i++) {
        if(array2[i-1]<array2[i]) {   
            x=i;
            c++;    
        }
        else {
            x=0;

            for(int j=0;j<array2.length-i;j++) {
                if(array2[j]>array2[j+1]) {
                    k=array2[j+1]; 
                    array2[j+1]=array2[j]; 
                    array2[j]=k;
                }
            }
        }
        JOptionPane.showMessageDialog(null,"La temperatura: "+array2[MAX-1]+" Día: "+(x-1));
    }
}
~~~

### Estudiando las variables locales

[Creación de variables locales en el Codepad](https://i.imgur.com/Hp6w6ZD.png)

[Variables locales de tipo int en la clase Person](https://i.imgur.com/emWjRBU.png)

### Experimentando con los literales en el Codepad

[Literales en el Codepad](https://i.imgur.com/MfS1h0e.png)

### Experimentando con operaciones en el Codepad

- El **operador módulo** da como resultado el resto de la división entera.

[Operaciones en el CodePad](https://i.imgur.com/Q54gkKE.png)

### Investigando la precedencia entre operaciones

~~~
8 + 2 * 2; 
8 + 4;          La multiplicación tiene precedencia en la operación
12 
~~~

~~~
4 - 6 / 2;
4 - 3;          La división tiene precedencia en la operación
1
~~~

- La **precedencia de operaciones** determina el orden en el cual los operadores son evaluados uno respecto al otro.

- En Java, la precedencia de operadores es:

1). Multiplicación y división.

2). Suma y resta.

3). Operadores lógicos (AND > XOR > OR > AND booleano)

### Fijando cómo se escribe el operador "igual que"

- El error más común que cometen aquellos que comienzan a programar en Java es confundir el **operador de asignación =** con el **operador relacional ==**.

- Otro error muy común es utilizar el **operador relacional ==** para comparar objetos de tipo _String_.

### Escribiendo código: constructor de Person en digital

- Un **gist** es una forma que se tiene para poder compartir código que **no sea demasiado grande** usando GitHub. Funciona igual que un repositorio, pudiendo **clonarlo**, **editarlo** y **comentarlo**.

[Crear nuevos gist](https://gist.github.com/)

[Constructor de Person](https://gist.github.com/JesusRiestra/8b023868635e98166e4f897099126389)

### Escribiendo código: métodos getter y setter de Person en digital

[Método getter y setter de Person](https://gist.github.com/JesusRiestra/ddb341e8f4ca6359d38d0e7da5e915db)

### Escribiendo más código en digital

[Más trozos de código](https://gist.github.com/JesusRiestra/fd6067f0f4c5c737e77e4ec044eb28f6)

### Entendiendo el concepto de interfaz de una clase

**Interfaz gráfica:** software que permite la interacción con la máquina de manera gráfica, con elementos como botones, ventanas o iconos.

**Interfaz de clase:** conjunto de todos los constructores y métodos públicos que un objeto pone a disposición de otros objetos.

### Entendiendo el uso de this

[Escenario 1](https://i.imgur.com/CShLs0l.png)

[Esceneario 2](https://i.imgur.com/mcX10Gc.png)

### Entendiendo las clases genéricas

Una **declaración** de un **atributo** privado llamado **librosBiblioteca** que sea de **tipo ArrayList** y que pueda contener objetos de la **clase Libro**:
~~~
private ArrayList<Libro> librosBiblioteca;
~~~

Cómo **inicializarías** el atributo del punto anterior **sin usar el operador diamante**:
~~~
librosBiblioteca = new ArrayList<Libro>();
~~~

Una **declaración** de una **variable local** llamada **curso** que pueda contener una colección de **objetos Alumno**:
~~~
ArrayList<Alumno> curso;
~~~

Cómo **inicializarías** la **variable local** del punto anterior **sin usar el operador diamante**:
~~~
curso = new ArrayList<Alumno>();
~~~

Una **declaración** de un **atributo** privado llamado **tracks** que pueda contener una colección de objetos de la **clase MusicTrack**:
~~~
private ArrayList<MusicTrack> tracks;
~~~

Como inicializarías el atributo del punto anterior usando el operador diamante:
~~~
tracks = new ArrayList<>();
~~~

### ArrayList: uso de la clase - Ahora se informa si un indice es válido

- El proyecto tiene 1 commit (Proyecto finalizado).

### Uso de clases de test ya creadas en BlueJ - Commit inicial

[Fallo al pasar los tests del método esMultiploDe2](https://i.imgur.com/ly1riDK.png)

[Fallo al pasar los tests del método esMultiploDe5](https://i.imgur.com/xB4lWxC.png)

[Fallo al pasar los tests del método esMultiploDe](https://i.imgur.com/qaXsV1j.png)

### Bucle for-each: procesamiento completo y selectivo de colecciones - Investigando los métodos de los ArrayList

[Captura 1](https://i.imgur.com/1MMR5kw.png)

### Características importantes de los objetos String - Investigando el método trim

public String trim() --> Devuelve un String cuyo valor es el propio String, con todos los espacios eliminados.

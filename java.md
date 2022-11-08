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
| a | Operador | b | Significado |
| a | Operador | b | Significado |
| a | Operador | b | Significado |
| a | Operador | b | Significado |
| a | Operador | b | Significado |
| a | Operador | b | Significado |





















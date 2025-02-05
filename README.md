# Aprendiendo a programar en C
A continución se encuentra el trabajo práctico que realicé en la materia "Arquitectura y Organización del Computador". El mismo tiene como objetivo la programación en C. 

----------------------------------------------------------------...----------------------------------------------------------------

# Un poco de C

Vamos a hacer uso de algunos de los conceptos vistos durante esta primer clase. En la carpeta _src_ van a encontrar unos cuantos archivos:

- `ej1.h`: contiene las declaraciones de variables y funciones a ser definidas en ej1.c.
- `ej1.c`: contiene las definiciones de las variables y funciones declaradas en ej1.h, algunas de las cuales deberán completar (ver enunciado más adelante).
- `main.c`: acá pueden definir sus propias pruebas, recuerden que todo programa en C comienza su ejecución llamando a la funcion _main_.
- `test.c`: contiene un caso de prueba. No se supone que lo modifiquen, pueden inspirarse en sus contenidos para realizar sus propias pruebas.
- `Makefile`: contiene las definiciones de **comandos de compilación**, para no tener que escribir el comando completo cada vez que se quiera compilar. Se invocan escribiendo **make** seguido de la etiqueta correspondiente (ej: `make all`, `make main`, `make test`).
- `runMain.sh`: script que compila y corre con valgrind su solución a partir de main.c.
- `runTester.sh` script que compila y corre con valgrind su solución a partir de test.c, comparando la salida producida con la salida esperada.
- `salida.catedra.txt`: archivo de salida generado por nuestra solución, contra el que se comparará el archivo que genere su solución al correr el archivo runTester.sh.

## Enunciado

OrgaLibre es una tienda online de componentes de PC que vende a precios muy bajos. Como quieren asegurarse de que sus clientes les vayan a dar buen uso a lo que compren, envían el catálogo de productos de una forma muy particular.

El catálogo se representa como un array de enteros de 32 bits donde cada par de elementos consecutivos almacena los datos de dos productos distintos de la siguiente forma:

![Esquema del catálogo](img/esquema-catalogo.png)

Entero 1: ID1 (8 bits), ID2 (8 bits), Precio1 (12 bits), Moneda1 (1 bit), Precio2 (bits 11 a 9)

Entero 2: Precio2 (bits 8 a 0), Moneda2 (1 bit), Stock1 (11 bits), Stock2 (11 bits)

Se pide:
1. Implementar las funciones `imprimir_producto` y `procesar_e_imprimir_catalogo` para ayudar a leer el catálogo cómodamente. Sus definiciones y detalles los van a encontrar en `ej1.h`





# First EDA Practice
Tomando un bloque de datos binarios de la memoria de un buzón de correos, se espera poder descifrar los correos que ya han sido borrados.
Los correos se envíaban codificados con un algoritmo al que sí que tenemos acceso.
Conociendo la dirección de correo y el algoritmo de ofuscación, este programa encuentra los correos que se encuentran en el fichero binario<.
<br> EDA1: <br>
El archivo se desencripta con cada una de las claves y se va probando si está el String buscado. Tiempos:
Prueba1.mbx: 8 segundos.
Prueba2.mbx: 1m. 20segundos

<br> EDA1EX <br>
Se cambia la perspectiva. Ahora se encripta el string buscado con cada una de las claves y se busca donde aparece en el texto.
En caso de que aparezca, se desencripta el fichero con una clave que hay que calcular según la posición donde se encuentre el texto buscado.
Tras esto, se vuelve a encriptar el fichero y se sigue buscando con el string encriptado con otra clave. Tiempos:
Prueba1.mbx: 2 segundos.
Prueba2.mbx: 15 segundos.
La diferencia de tiempo es abismal en tamaños grandes de archivos.

#Créditos:
Esta práctica es la primera y está realizada para la asignatura Estructura de Datos y Algoritmos, impartida por Cesar Vaca en la UVa.
Elaborado por: 
- Javier @Helguera
- Álvaro Velasco (@Velastroll)

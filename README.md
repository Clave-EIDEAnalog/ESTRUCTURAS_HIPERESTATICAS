# ESTRUCTURAS_HIPERESTATICAS
Esta página WEB recoge una serie de problemas de resolución de estructuras hiperestáticas por el método de la flexibilidad. Los problemas -la mayor parte- se han extraído de la asignatura Estructuras 2 del Grado de Arquitectura de la escuela Politécnica de Zaragoza (UZ).
No se incluye la teoría básica para la resolución de los problemas, que el lector deberá conocer. El objetivo de esta colección de problemas es la clasificación y análisis de los mismos para su mejor comprensión por parte del alumno; no obstante, en algún momento se hace alguna consideración teórico-práctica, siempre que ésta redunde en beneficio de la comprensión de la resolución de los problemas. 
La mayor parte de los problemas son, o bien de _examen_ en cursos anteriores al 2022 – 2023, o bien realizados en clase durante el citado curso. También se han incluido algunos problemas a título de enlace entre los anteriores cuando se ha entendido interesante para lograr una complicación progresiva de los mismos; buena parte de ellos se han sacado del libro de problemas _Cegoñino_(CG).
Además de las fuentes citadas, se hace referencia a veces al -excelente- texto de la UPC “Mecánica de estructuras II. Métodos de análisis (Miguel Cervera Ruiz -UPC-)”, sobre todo para analizar alguno de los problemas resueltos -ejemplos- que incluye.

**NOTA IMPORTANTE**: Las soluciones a los problemas están redactados a mano y son ficheros (los PDF que las contienen) extensos. Si la página ni deja verlos simplemente _pinchando_ en el nombre del fichero, dar a "Download" 


![INDICE_I](https://user-images.githubusercontent.com/64075009/218720476-a7913e48-b19f-4b49-83da-325d4476bcbc.jpg)
![INDICE_Ib](https://user-images.githubusercontent.com/64075009/218721461-33e98d48-dd33-4aa3-b13d-b72f93ed4673.jpg)
![INDICE_II](https://user-images.githubusercontent.com/64075009/218722984-df270c18-3aed-41fd-84d1-774827b33e14.jpg)
![INDICE_IIb](https://user-images.githubusercontent.com/64075009/218722998-338de010-d793-4cc1-95cc-363ca8cb4bdd.jpg)
![INDICE_III](https://user-images.githubusercontent.com/64075009/218723017-c45970d5-b479-4d98-8367-132c48b99940.jpg)
![MEFI_25](https://user-images.githubusercontent.com/64075009/221239689-c2c6dde6-4886-4652-b988-f2000be26089.png)

## Estructuras articuladas.
### Estructuras resolubles utilizando solamente las deformaciones.
(Problemas 2, 10 y 14)
Son los casos más simples y pueden resolverse mediante, sólamente, el análisis de las deformaciones (método de la compatibilidad, flexibilidad, compatibilidad/flexibilidad). Algunos están resueltos también por aplicación del PTV y son un buen ejercicio de este método.
Nivel de complicación:
14 → 2 → 10. 


## Estructuras a las que es conveniente aplicar el PTV.
### Cálculo de deformaciones (movimientos de nudos) en estructuras NO hiperestáticas.
El PTV es un principio genérico de comportamiento de una estructura elástica, por lo que ni está restringido a la resolución de estructuras hiperestáticas ni, solamente, al cálculo de desplazamientos (ni, por tanto, al cálculo de desplazamientos en estructuras hiperestáticas).
El problema 16 no es una estructura hiperestática, pero se incluye como práctica de la aplicación del PTV a las estructuras articuladas.

### Cálculo de estructuras hiperestáticas.
Casi todas las estructuras hiperestáticas se pueden resolver por el método de la compatibilidad (flexibilidad, compatibilidad/flexibilidad), pero a medida que se complica la estructura lo hace el número de nodos y, por tanto el de ecuaciones a plantear, hasta tal punto que, a pesar de lo farragoso (también) de su aplicación, es conveniente usar el PTV.
Para la aplicación de éste es conveniente seguir a rajatabla los siguientes puntos:
- Salvo que se trate de una esturcura muy simple y la forma de trabajo de TODAS sus barras (tracción vs. compresión; tanto en el sistema isostático como en el virtual) obvia, es conveniente suponer de entrada que todas las barras trabajan a tracción: el signo de los productos de los alargamientos por las tensiones, que a veces no se sabe hasta que se resuelve numéricamente el problema, es muy importante para la aplicación del PTV.
- Inevitablemente la aplicación del PTV conduce a desarrollos algebráicos farragosísimos, por lo que la 'limpieza' (simplificacion de las expresiones que aparecen en la tabla) de la tabla es fundamental para resolver completamente el problema.
- Precisamente por esta razón (lo complicado de llegar a la solución numérica sin confundirse), se suele calificar un problema como bien resuelto si se llega a plantear la tabla, por lo que es vital entender como se construye y aplica.

El PTV tiene una demostración en la que se manejan conceptos matemáticos de cierta complejidad; si bien su uso es más una cuestión de técnica que de concepto (que también lo tiene), para desenvolverse mínimamente con la herramienta hay que resolver un número de problemas. Se aconseja la siguiente secuencia:

16 → 2 → 5 → 4 → 3 → 18 → 17 → 11 → 19


## Uso de MEFI y Excel como herramientas auxiliares.

### MEFI
Es utilísimo, no solamente para comprobar la solución numérica final, sino para ir verificando los cálculos a medida que se van, por ejemplo, resolviendo los nudos (y obteniendo las expresiones parciales de tensiones reales -y virtuales).
En los problemas en los que no se especifican los valores de A y E (y posteriormente, en las estructuras en las que hay flexión "I") se ve como se suele tomar como "A" el valor 4,762xE-N (lo mismo -no _el mismo_- para "I") y "1" para las longitudes. La razón es que el producto de estos valores por el de "E" del acero (2xE11 Pa) da multiplo de 10 y con un vistazo a las soluciones de MEFI se pueden comprobar hasta cuatro cifras significativas de lo que se va haciendo. Así, por ejemplo, si un valor parcial nos sale 1/2 (_a mano_), MEFI nos dará 0,5 Ex (o 0,4999 Ex) si es correcto.

### Excel
Aunque en mucha menor medida que MEFI, en problemas con desarrollos algebráicos muy compilicados se puede usar excel para verificar que, al menos, un valor cumple una determinada ecuación (lo que, a veces, no es poca cosa. Es necesario, eso sí, manejar excel con soltura)


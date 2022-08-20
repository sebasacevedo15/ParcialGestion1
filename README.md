# ParcialGestion1
Parcial Juan Sebastian Acevedo Gestion de datos
########


###################Se sube otro readme en formato txt para el caso que los datos en las respuestas no se puedan ver con las tabulaciones realizadas

1. Tipos de variables
gender                          object	Categórica nominal
race/ethnicity                  object	Categórica nominal
parental level of education     object	Categórica ordinal
lunch                           object	Categórica nominal
test preparation course         object	Categórica nominal
math score                     float64	Escalar continua
reading score                  float64	Escalar continua
writing score                  float64	Escalar continua

Se encuentra que las variables tienen el formato autoasignado correcto.

2. Calidad de los datos
  -Inicialmente se encuentra que en todas las columnas hay datos nulos.
  -Se eliminan las columnas con datos nulos, para facilidad del ejercicio analítico
  

3. La materia con mejor promedio es:
Promedio en reading:
69.54
Al análizar la distribución de datos de las notas de reading se encuentra una asimetría negativa, mostrando que la mayoría de los estudiantes resultados altos y que solo se encuentran unos pocos (registros atipicos) con un resultado muy bajo.
Igualmente se observa que esta variable tiene una distribución muy similar a la curva normal, es decir los datos estan normalizados en un buen nivel

4. Se encuentran correlaciones muy altas entre las tres variables de al menos un 80%

               math score  reading score  writing score
math score       1.000000       0.821609       0.806391
reading score    0.821609       1.000000       0.956514
writing score    0.806391       0.956514       1.000000

Lo cual indica que en general los estudiantes con una nota alta en algun examen tuvo igualmente notas altas en las otras asignaturas


5.Al realizar análisis de los promedios obtenidos por genero, no se encuentra un género que en general tenga mejor promedio en todas las asignaturas. Pero se puede defir que en math los estudiantes con género no binario tienen mejor puntaje, en reading lo tienen el género femenino y en writing lo tiene igualmente el género femenino. El genero masculino no se aleja notablemente del promedio. 

6.Se toma la muestra del df original filtrando sólo los valores mayores en calificación de lectura para el percentil 85
Se encuentra una muestra de 97 estudiantes con esta condición 

Con esto se analiza el nivel de escolaridad de los padres obteniendo:
associate's degree    26.804124
some college          21.649485
bachelor's degree     18.556701
some high school      15.463918
master's degree       10.309278
high school            7.216495

associate's degree es el nivel de escolaridad que mayor tienen los padres en promedio para este grupo de estudiantes.

7.Se encontró que sólo 21 estudiantes tienen calificaciones mayores o iguales a 90 en ambas asignaturas, de los cuales se encuentra la siguiente distrobución

Frec Absoluta
completed    12
none          9

Fre Relativa
completed    57.142857
none         42.857143

El 57,14% de los estudiantes con notas mayor a 90 completaron el curso de preparación para el examen.

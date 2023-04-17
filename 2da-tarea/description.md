# 🧹🧩 Tarea 2: limpieza y modelado de datos 🗃️

Una vez obtenida una buena comprensión del proyecto y mi función en él, ¡es hora de ponerse a trabajar!

Entonces, debo echar un vistazo a los datos con los que trabajar. El cliente ha enviado:

+ <strong>Siete datasets</strong>: cada conjunto de datos contiene diferentes columnas y valores.
+ <a href='./Data model.pdf'>Un modelo de datos</a>: este muestra las relaciones entre todos los conjuntos de datos, así como los enlaces que se pueden usar para fusionar las tablas.

Hay mucha información de momento y es fácil perderse en los datos. Entonces, para asegurarme de que estoy utilizando los datos correctos para responder a los objetivos, debo seguir los siguientes pasos:

+ Recopilación de requisitos.
+ Limpieza de datos.
+ Modelado de datos.

## Primero, recopilación de requisitos 🕵🏻‍♀️

No necesitaré todos los conjuntos de datos para encontrar lo que estoy buscando.

Por lo tanto, el primer paso es usar el modelo de datos para identificar qué datasets se requerirán para descubrir las cinco categorías principales con la mayor popularidad.

Cuando identifique los conjuntos de datos correctos para incluir, completaré una breve verificación de conocimientos, para luego pasar al siguiente paso.

<strong>Resolución</strong>:

Los 3 datasets necesarios para avanzar son:
+ <strong>Reaction</strong>
+ <strong>Content</strong>
+ <strong>Reaction Types</strong>

<strong><font color="#8AB8BB">Mi trabajo es identificar qué categorías de contenido son las más populares. La popularidad se determina en función de las puntuaciones de reacción.</font></strong>


Antes de comenzar a trabajar con los datasets, debo asegurarme de que los datos estén limpios y listos para el análisis..

## Limpieza de datos 🧹

La limpieza de datos es una etapa anterior al modelado que se centra en la detección y corrección de errores o inconsistencias en los datos, como valores faltantes o datos duplicados.

<strong>Objetivos</strong>:

+ Eliminar filas con valores faltantes.
+ Cambiar los nombres de ciertas columnas.
+ Cambiar el tipo y formato de datos de ciertas columnas.
+ Eliminar columnas que sean irrelevantes para esta tarea.
 
El resultado final deben ser tres datasets limpios. 

<a href='./data-cleaning.ipynb'>Ir al cuaderno</a>

## Modelado de datos 🧩

Para hacer el modelado de datos, se deben seguir los siguientes pasos:
1. Crear un dataset final fusionando las tres tablas.
Se recomienda usar la tabla `Reaction` como tabla base: primero se deben unir las columnas relevantes del dataset `Content` y luego  de `Reaction Types`.
1. Averiguar las 5 categorías con mayor popularidad. Para esto sumar las puntuaciones totales de cada categoría.

El resultado final debe ser:
+ Un dataset limpio.
+ Las 5 categorías principales.
  
<a href='./data-modelling.ipynb'>Ir al cuaderno</a>

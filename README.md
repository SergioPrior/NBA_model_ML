# Nba_Presupuesto_Salarios.

![image](https://github.com/SergioPrior/NBA_model_ML/assets/158041668/64ac11a1-1ec1-494c-8471-64a930770276)

# Presupuesto y salarios NBA
## 1 - Descripción
Los datos de este proyecto han sido scrapeados de las páginas:
- NBA Reference (https://www.basketball-reference.com/)
- Hispanos NBA (https://www.hispanosnba.com/)

El proyecto está basado en el análisis de las estadísticas de los jugadores para predecir, según su rendimiento en la temporada actual, el salario que deberían adquirir.

Para ello, se han realizado los siguientes pasos:

## 2 - Objetivos de desarrollo
### 2.1 - Análisis exploratorio
El principal objetivo es investigar las páginas web y el método de scrapeo. Una vez realizado mediante BeautifulSoup (BS4), procedemos a la importación de los datos a nuestro archivo ipynb.

### 2.2 - Limpieza de datos
Comenzamos con la limpieza de los datos eliminando valores NaN, buscando errores en las tablas e implementando mejoras para la optimización de estas. Una vez tenemos los datos limpios, pasamos al tipo de dato que necesitamos para trabajarlo con homogeneidad.

### 2.3 - Unión de los datos
Una vez limpio cada CSV scrapeado, comenzamos con la unión de las tablas utilizando los diferentes métodos que nos facilita el lenguaje de Python (merge, concat, join, etc.). Después de esto, y muy importante, realizamos la comprobación de que todo se ha unificado correctamente sin habernos dejado ningún dato por el camino o que se hayan creado valores NaN que nos puedan poner problemas en el desarrollo del modelo.

## 3 - Predicción
Entrenar el modelo capaz de predecir el salario de los jugadores en base a su rendimiento, utilizando las variables que puedan repercutir a la hora de cobrar el sueldo. A mejor puntuación, mejor salario. Hemos usado métodos como "Features Importances" para ver la colinealidad de dichas variables.

## 4 - Uso
Todo el proceso lo tenéis disponible en este enlace (https://github.com/SergioPrior/NBA_model_ML), donde podéis encontrar las carpetas:
- [NBA_csv](https://github.com/SergioPrior/NBA_model_ML/tree/main/NBA_csv)
- [src](https://github.com/SergioPrior/NBA_model_ML/tree/main/src)

Aquí tenéis todo lo necesario para aquellos que tengan alguna curiosidad sobre las librerías o el código que he usado, o para recrear el proyecto y, quién sabe, mejorarlo aún más.

## 5 - Conclusiones
Finalmente, después del estudio realizado, hemos llegado a la conclusión de que tenemos un fuerte emparejamiento de la edad con el salario, debido a los jugadores "rookies" de la liga.
- Hay claramente una diferencia salarial muy grande entre lo que cobran los recién llegados y los que tienen ya veteranía en el sector, aunque los jugadores con menos experiencia estén jugando al nivel de un veterano, su salario es menor debido a la edad que tienen.
- Hemos podido ver cómo los mejores contratos se consiguen a raíz de los 25 años en adelante y su bajada la tienen a partir de los 35 años, excepto si eres un LeBron James.
- Por último, el rendimiento de los jugadores veteranos, ya sea por una lesión o por una mala temporada, afecta al salario real que están cobrando. El modelo nos ayuda a ver qué jugador actualmente, en base a su rendimiento, debería ser su salario, ya que pueden estar jugando como un recién llegado.

## 6 - Next steps
Los próximos pasos son identificar más variables externas al juego para poder predecir con más exactitud el resto de sus ingresos salariales. Buscaremos variables relacionadas con la participación en el All-Star, número de contratos firmados y su duración, y también sus derechos de imagen o anillos conseguidos.




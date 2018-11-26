# Gauss Seidel

En análisis numérico el método de Gauss-Seidel es un método iterativo utilizado para resolver sistemas de ecuaciones lineales. El método se llama así en honor a los matemáticos alemanes Carl Friedrich Gauss y Philipp Ludwig von Seidel y es similar al método de Jacobi.

Aunque este método puede aplicarse a cualquier sistema de ecuaciones lineales que produzca una matriz (cuadrada, naturalmente pues para que exista solución única, el sistema debe tener tantas ecuaciones como incógnitas) de coeficientes con los elementos de su diagonal no-nulos, la convergencia del método solo se garantiza si la matriz es diagonalmente dominante o si es simétrica y, a la vez, definida positiva.

La secuencia de pasos que constituyen el método de Gauss-Seidel es la siguiente:

1. Asignar un valor inicial a cada incógnita que aparezca en el conjunto. Si es posible hacer una hipótesis razonable de éstos valores, hacerla. Si no, se pueden asignar valores seleccionados arbitrariamente. Los valores iniciales utilizados no afectarán la convergencia como tal, pero afectarán el número de iteraciones requeridas para dicha convergencia.
2. Partiendo de la primera ecuación, determinar un nuevo valor para la incógnita que tiene el coeficiente más grande en esa ecuación, utilizando para las otras incógnitas los valores supuestos.
3. Pasar a la segunda ecuación y determinar en ella el valor de la incógnita que tiene el coeficiente más grande en esa ecuación, utilizando el valor calculado para la incógnita del paso 2 y los valores supuestos para las incógnitas restantes.
4. Continuar con las ecuaciones restantes, determinando siempre el valor calculado de la incógnita que tiene el coeficniente más grande en cada ecuación particular, y utilizando siempre los últimos valores calculados para las otras incógnitas de la ecuación. (Durante la primera iteración, se deben utilizar los valores supuestos para las incógnitas hasta que se obtenga un valor calculado). Cuando la ecuación final ha sido resuelta, proporcionando un valor para la única incógnita, se dice que se ha completado una iteración.
5. Continuar iterando hasta que el valor de cada incógnita, determinado en una iteración particular, difiera del valor obtenido en la iteración previa, en una cantidad menor que cierto EPSILON seleccionado arbitrariamente. El procedimiento queda entonces completo.

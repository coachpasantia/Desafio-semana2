# Desafios de la semana.

## Desafio 1
1. principiante:
👩‍💻 estás trabajando en un sistema operativo para ser usado en el taller de Santa Claus 🎅.

Se ha dado cuenta que en el taller nadie le presta atención a los nombres de los ficheros y a veces intentan guardar el mismo fichero más de una vez... así que es importante que gestionemos bien los nombres duplicados.

Tenemos que crear una función que al pasarnos un array de nombres de archivo devolvamos un array con el mismo número de elementos pero donde los nombres que se repetían se anexe al final (k) donde k sería el número de veces que se encontró repetido.

Lo mejor es que veamos un ejemplo:

```python
files = ['photo', 'postcard', 'photo', 'photo', 'video']
fixFiles(files) # ['photo', 'postcard', 'photo(1)', 'photo(2)', 'video']

files2 = ['file', 'file', 'file', 'game', 'game']
fixFiles(files2) = ['file', 'file(1)', 'file(2)', 'game', 'game(1)']

# ojo que los elfos ya tenían archivos con (1)... ¡y pueden estar repetidos!
files3 = ['file', 'file(1)', 'icon', 'icon(1)', 'icon(1)']
fixFiles(files3) # ['file', 'file(1)', 'icon', 'icon(1)', 'icon(1)(1)']
```

## Desafio2

2. Intermedio:
¡Estamos haciendo los últimos ajustes para el trineo de Santa Claus!

Como ya sabes, el trineo es volador y estamos ajustando el motor para que haga parabolas lo más óptimas posibles. Para esto el salto debe ser siempre hacia arriba y, a partir del punto más alto, debe bajar siempre hacia abajo...

Nuestro mecánico de confianza, Kiko Belfs, que tiene un Tesla genial, nos ha explicado que los saltos se pueden ver como arrays... y que sólo tenemos que asegurarnos que los números suben y bajan de forma correcta. También nos avisa que sólo pasaremos arrays de, como mínimo, tres posiciones.

Nos ha pasado algunos ejemplos de cómo debería ser nuestra función y algunos resultados:
```python
checkSledJump([1, 2, 3, 2, 1]) # true: sube y baja de forma estricta
checkSledJump([0, 1, 0]) # -> true: sube y baja de forma estricta
checkSledJump([0, 3, 2, 1]) # -> true: sube y baja de forma estricta
checkSledJump([0, 1000, 1]) # -> true: sube y baja de forma estricta

checkSledJump([2, 4, 4, 6, 2]) # false: no sube de forma estricta
checkSledJump([1, 2, 3]) # false: sólo sube
checkSledJump([1, 2, 3, 2, 1, 2, 3]) # false: sube y baja y sube... ¡no vale!
```

## Desafio 3
3. intermedio
Para mejorar la productividad de la tienda en la que trabajamos, vamos a crear una pequeña máquina que calcula el mínimo número de monedas que debemos usar para dar el cambio de una compra en metálico.

Las monedas para cambio que puedes usar son estas:
```python
coins[0] = 1 céntimo
coins[1] = 2 céntimos
coins[2] = 5 céntimos
coins[3] = 10 céntimos
coins[4] = 20 céntimos
coins[5] = 50 céntimos
```
Tenemos que crear una función que recibe el número de céntimos que hay que devolver al cliente y la función nos da un array con la combinación de monedas mínimas que debemos usar para conseguirlo.

```python
getCoins(51) # [1, 0, 0, 0, 0, 1] -> una moneda de 1 céntimo y otra de 50 céntimos
getCoins(3) # [1, 1, 0, 0, 0, 0] -> una moneda de 1 céntimo y otra de 2
getCoins(5) # [0, 0, 1, 0, 0, 0] -> una moneda de 5 céntimos
getCoins(16) # [1, 0, 1, 1, 0, 0] -> una moneda de 1 céntimo, una de 5 y una de 10
getCoins(100) # [0, 0, 0, 0, 0, 2] -> dos monedas de 50 céntimos
```# Desafio-semana2

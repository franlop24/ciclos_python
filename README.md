# Ciclos en Python

## Ciclo for

Es una estructura iterativa en la que se puede definir el número de veces que una intrucción se va a ejecutar.

Ejemplos:
- Programa que imprima los números del 1 al 10
- Programa que muestre 5 veces la frase "Hola Mundo!"

### Estructura

```
for variable in rango:
    instrucciones
```
Donde:
- variable: valor que va cambiando en cada iteración
- rango: de donde a donde va el ciclo

Para definir un rango se utiliza la función range()
- range(n): [0, ..., n - 1]
range(5): [0, 1, 2, 3, 4]
- range(ini, n): [ini, ini + 1, ini + 2, ... , n - 1]
range(2, 8): [2, 3, 4, 5, 6, 7]
- range(ini, n, step): [ini, ini + step, ..., n - 1]
range(0, 10, 2): [0, 2, 4, 6, 8]

## Ciclo while
Es una estructura de control que se utiliza para ejecutar un grupo de instrucciones de forma repetida mientras que se cumpla una condición

Ejemplos:
- Imprimir números mientras sean menores a 10
- Obtener el factorial de un número: multiplicar por n - 1 mientras sea mayor o igual a 1

El Ciclo While tiene 2 implementaciones:
- En la primera evalua una expresión para ver si ejecutará las instrucciones, este puede que no las ejecute ninguna vez
- En la segunda primero ejecuta las instrucciones y después evalúa una expresión, en este al menos una vez se van a ejecutar las instrucciones (Do While)

### Estructura
while
```
while exp_booleana:
    instrucciones
```
Donde:
La expresión booleana será la que determine si se ejecutan las instrucciones.
Dentro del bloque de instrucciones se deben ir actualizando los valores que se evalúan en la expresiín booleana para asegurar que no se termine en un ciclo infinito

Do While
```
while True:
    instrucciones
    if exp_booleana:
        break
```
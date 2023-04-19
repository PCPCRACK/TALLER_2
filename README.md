# TALLER_2
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"
## "TODOS LOS PUNTOS DEBEN TENER UNA FUNCION MINIMO"

#Nombres Integrantes: PD: escriban sus names.

 
 * David Andres Rojas Villarreal.
 *
 *

1. Desarrollar un programa que ingrese un número entero n y separe todos los digitos que componen el número.
2. Desarrollar un programa que ingrese un número flotante n y separe su parte entera de la parte decimal, y luego entrege los digitos tanto de la parte entera como de la decimal.
```python
#llama una libreria y importa una funcion
from math import modf 

def Sep(n : float):

    #retorna el valor de una funcion dentro de otra funcion
    return modf(n)


if __name__ == "__main__":
    
    #pide un valor flotante
    n = float(input("ingrese un numero con decimales: "))

    #crea una lista vacia
    lista = list()

    #llama una funcion y almacena la informacion que retorna la funcion en la lista
    lista = Sep(n)

    #imprime los resultados
    print(f"su parte entera es {(lista[1])} y su decimal {(lista[0])} numero inicial {n}")
```



3. Desarrollar un programa que permita ingresar dos números enteros y determinar si se tratan de números espejos.
4. Diseñar una función que permita calcular una aproximación de la función coseno alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Taylor. **nota:** use *math* para traer la función coseno y mostrar la diferencia entre el valor real y la aproximación. Con cuántos valores de la serie, se tienen errores del 10%, 1%, 0.1% y 0.001%.
$$cos(x) \approx cos(x,n) \approx \sum_{i=0}^{n} (-1)^i \frac{x^{2i}}{(2i)!}$$
5. Desarrollar un programa que permita determinar el Minimo Comun Multiplo de dos numeros enteros. Abordar el problema desde la perpectiva iterativa como recursiva.
```python
def Minc(n : int,a : int,i : int):

  # Caso base 
  if i%n == 0 and i%a == 0 : 
    return i
  else:
    # Condicion de la funcion recursiva
    return Minc(n,a,i+1)

if __name__ == "__main__":
  n = int(input("Ingrese un numero: "))
  a = int(input("Ingrese un numero: "))
  i = 2

  #llama la funcion
  Minc = Minc(n,a,i)

  #imprime los resultados
  print(f"el minimo comun multiplo de los numeros {n} y {a} es {Minc}")

```

6. Desarrollar un programa que determine si en una lista no existen elementos repetidos.
7. Desarrollar un programa que determine si en una lista se encuentra
una cadena de caracteres con dos o más vocales. Si la cadena existe debe imprimirla y si no existe debe imprimir 'No existe'.
8. Desarrollar un programa que dadas dos listas determine que elementos tiene la primer lista que no tenga la segunda lista. **Ejemplo:**
<center>
<table border="1">
<tr>
<td>
lista1: [1, 'Hola', -12.3 ,True]<br>
lista2: [11, -12.3, 'Hola', False]
</td>
</tr>
<tr>
<td>
salida: [1, True]
</td>
</tr>
</table>
</center>

9. Resolver el punto 7 del [taller 1](https://github.com/fegonzalez7/pdc_unal_clase8) usando operaciones con vectores.

10. Desarrollar un algoritmo que determine si una matriz es mágica. Se dice que una matriz cuadrada es mágica si la suma de cada una de sus filas, de cada una de sus columnas y de cada diagonal es igual.

# Cristian Gómez
# Isabella Moreno
# Juan Rey
# Taller-1
#Puntos impares
# 3.Realice un programa que lea un número enteros y determine si es par o impar.
x : int
x = int(input("Ingrese un número entero "))
if x % 2 == 0:
    print("El número " + str(x) + " es par")
else:
    print("El número " + str(x) + " no es par")
# 5.Realice un programa que lea tres números reales y determine si la suma de los dos primeros es mayor, menor o igual que el tercer número.
x : int
x = int(input("Ingrese el valor a "))
y : int
y = int(input("Ingrese el valor b "))
z : int
z = int(input("Ingrese el valor c "))
h : int = x + y
if x + y > z:
  print("La suma de " + str(x) + " y " + str(y) + " (" + str(h) + ") " "es mayor a " + str(z) + ".")
elif x + y < z:
   print("La suma de " + str(x) + " y " + str(y) + " (" + str(h) + ") " " es menor a " + str(z) + ".")
elif x + y == z:
   print("La suma de " + str(x) + " y " + str(y) + " (" + str(h) + ") " " es igual a " + str(z) + ".")
# 7. Escriba un programa que pida 5 números reales y calcule las siguientes operaciones:
El promedio La mediana El promedio multiplicativo (multilplica todos y luego calcula la raíz de la cantidad de operandos) Ordenar los números de forma ascendente Ordenar los números de forma descendente La potencia del mayor número elevado al menor número La raíz cúbica del menor número   
x : int
x = int(input("Ingrese el valor 1: "))
y : int
y = int(input("Ingrese el valor 2: "))
z : int
z = int(input("Ingrese el valor 3: "))
n : int
n = int(input("Ingrese el valor 4: "))
i : int
i = int(input("Ingrese el valor 5: "))
h : int = (x + y + z + n + i)/5
g : int = (x * y * z * n * i) ** 0.5

print("El promedio de los datos es: " + str(h) + "." )
#Para calcular la mediana podemos utilizar la biblioteca numPy
import numpy as np

data = [ x, y, z, n, i]

median = np.median(data)

print("La mediana de los datos es:", median)
print("el promedio multiplicativo es " + str(g) + ".")


#Ordenar los valores de forma ascendente y resultados
if x < y < z < n < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif x < y < z < i < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n))
elif x < y < n < z < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif x < y < n < i < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif x < y < i < z < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n))
elif x < y < i < n < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z))
elif x < z < y < n < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i))
elif x < z < y < i < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n))
elif x < z < n < y < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i))
elif x < z < n < i < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y))
elif x < z < i < y < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n))
elif x < z < i < n < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y))
elif x < n < y < z < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i))
elif x < n < y < i < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z))
elif x < n < z < y < i:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i))
elif x < n < z < i < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y))
elif x < n < i < y < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z))
elif x < n < i < z < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y))
elif x < i < y < z < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n))
elif x < i < y < n < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z))
elif x < i < z < y < n:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n))
elif x < i < z < n < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y))
elif x < i < n < y < z:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z))
elif x < i < n < z < y:
    print("El orden ascendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y))
elif y < x < z < n < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif y < x < z < i < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n))
elif y < x < n < z < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif y < x < n < i < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif y < x < i < z < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n))
elif y < x < i < n < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z))
elif y < z < x < n < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i))
elif y < z < x < i < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n))
elif y < z < n < x < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i))
elif y < z < n < i < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x))
elif y < z < i < x < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n))
elif y < z < i < n < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x))
elif y < n < x < z < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i))
elif y < n < x < i < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z))
elif y < n < z < x < i:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i))
elif y < n < z < i < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x))
elif y < n < i < x < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z))
elif y < n < i < z < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x))
elif y < i < x < z < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n))
elif y < i < x < n < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z))
elif y < i < z < x < n:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n))
elif y < i < z < n < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x))
elif y < i < n < x < z:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z))
elif y < i < n < z < x:
    print("El orden ascendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x))
elif z < x < y < n < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i))
elif z < x < y < i < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n))
elif z < x < n < y < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i))
elif z < x < n < i < y:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y))
elif z < x < i < y < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n))
elif z < x < i < n < y:
    print("El orden ascendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y))
elif z < y < x < n < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i))
elif z < y < x < i < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(n))
elif z < y < n < x < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i))
elif z < y < n < i < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x))
elif z < y < i < x < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n))
elif z < y < i < n < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x))
elif z < n < x < y < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i))
elif z < n < x < i < y:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y))
elif z < n < y < x < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i))
elif z < n < y < i < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x))
elif z < n < i < x < i:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(i))
elif z < n < i < i < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(i)+ ', ' +str(x))
elif z < i < x < y < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n))
elif z < i < x < n < y:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y))
elif z < i < y < x < n:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n))
elif z < i < y < n < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x))
elif z < i < n < x < y:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y))
elif z < i < n < y < x:
    print("El orden ascendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x))
elif n < x < y < z < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif n < x < n < i < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif n < x < z < n < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif n < x < z < i < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(y))
elif n < x < i < y < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z))
elif n < x < i < z < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y))
elif n < y < x < z < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i))
elif n < y < x < i < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z))
elif n < y < z < x < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i))
elif n < y < z < i < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x))
elif n < y < i < x < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z))
elif n < y < i < z < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x))
elif n < z < x < y < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i))
elif n < z < x < i < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y))
elif n < z < y < x < i:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i))
elif n < z < y < i < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x))
elif n < z < i < x < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y))
elif n < z < i < y < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x))
elif n < i < x < y < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z))
elif n < i < x < z < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y))
elif n < i < y < x < z:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z))
elif n < i < y < z < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x))
elif n < i < z < x < y:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y))
elif n < i < z < y < x:
    print("El orden ascendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x))
elif i < x < y < z < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n))
elif i < x < y < n < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z))
elif i < x < z < y < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n))
elif i < x < z < n < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y))
elif i < x < n < y < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z))
elif i < x < n < z < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y))
elif i < y < x < z < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n))
elif i < y < x < n < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z))
elif i < y < z < x < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n))
elif i < y < z < n < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x))
elif i < y < n < x < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(n)+ ', ' +str(z))
elif i < y < n < z < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x))
elif i < z < x < y < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n))
elif i < z < x < n < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y))
elif i < z < y < x < n:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n))
elif i < z < y < n < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x))
elif i < z < n < x < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y))
elif i < z < n < y < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x))
elif i < n < x < y < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z))
elif i < n < x < z < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y))
elif i < n < y < x < z:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z))
elif i < n < y < z < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x))
elif i < n < z < x < y:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y))
elif i < n < z < y < x:
    print("El orden ascendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x))


#Ordenar los valores de forma descendente y resultados
if x > y > z > n > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif x > y > z > i > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n))
elif x > y > n > z > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif x > y > n > i > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif x > y > i > z > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n))
elif x > y > i > n > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z))
elif x > z > y > n > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i))
elif x > z > y > i > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n))
elif x > z > n > y > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i))
elif x > z > n > i > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y))
elif x > z > i > y > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n))
elif x > z > i > n > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y))
elif x > n > y > z > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i))
elif x > n > y > i > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z))
elif x > n > z > y > i:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i))
elif x > n > z > i > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y))
elif x > n > i > y > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z))
elif x > n > i > z > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y))
elif x > i > y > z > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n))
elif x > i > y > n > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z))
elif x > i > z > y > n:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n))
elif x > i > z > n > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y))
elif x > i > n > y > z:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z))
elif x > i > n > z > y:
    print("El orden descendente es: " +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y))
elif y > x > z > n > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif y > x > z > i > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n))
elif y > x > n > z > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif y > x > n > i > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif y > x > i > z > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n))
elif y > x > i > n > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z))
elif y > z > x > n > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i))
elif y > z > x > i > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n))
elif y > z > n > x > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i))
elif y > z > n > i > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x))
elif y > z > i > x > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n))
elif y > z > i > n > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x))
elif y > n > x > z > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i))
elif y > n > x > i > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z))
elif y > n > z > x > i:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i))
elif y > n > z > i > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x))
elif y > n > i > x > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z))
elif y > n > i > z > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x))
elif y > i > x > z > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n))
elif y > i > x > n > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z))
elif y > i > z > x > n:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n))
elif y > i > z > n > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x))
elif y > i > n > x > z:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z))
elif y > i > n > z > x:
    print("El orden descendente es: " +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x))
elif z > x > y > n > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i))
elif z > x > y > i > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n))
elif z > x > n > y > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i))
elif z > x > n > i > y:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(y))
elif z > x > i > y > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n))
elif z > x > i > n > y:
    print("El orden descendente es: " +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y))
elif z > y > x > n > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i))
elif z > y > x > i > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(n))
elif z > y > n > x > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i))
elif z > y > n > i > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x))
elif z > y > i > x > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n))
elif z > y > i > n > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x))
elif z > n > x > y > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i))
elif z > n > x > i > y:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y))
elif z > n > y > x > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i))
elif z > n > y > i > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x))
elif z > n > i > x > i:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(i))
elif z > n > i > i > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(i)+ ', ' +str(x))
elif z > i > x > y > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n))
elif z > i > x > n > y:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y))
elif z > i > y > x > n:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n))
elif z > i > y > n > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x))
elif z > i > n > x > y:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y))
elif z > i > n > y > x:
    print("El orden descendente es: " +str(z)+ ', ' +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x))
elif n > x > n > z > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(i))
elif n > x > n > i > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(i)+ ', ' +str(z))
elif n > x > z > n > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(i))
elif n > x > z > i > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(y))
elif n > x > i > y > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z))
elif n > x > i > z > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y))
elif n > y > x > z > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(i))
elif n > y > x > i > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(z))
elif n > y > z > x > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i))
elif n > y > z > i > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x))
elif n > y > i > x > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z))
elif n > y > i > z > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x))
elif n > z > x > y > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(i))
elif n > z > x > i > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(i)+ ', ' +str(y))
elif n > z > y > x > i:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(i))
elif n > z > y > i > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(i)+ ', ' +str(x))
elif n > z > i > x > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y))
elif n > z > i > y > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(z)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x))
elif n > i > x > y > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z))
elif n > i > x > z > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y))
elif n > i > y > x > z:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z))
elif n > i > y > z > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x))
elif n > i > z > x > y:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y))
elif n > i > z > y > x:
    print("El orden descendente es: " +str(n)+ ', ' +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x))
elif i > x > y > z > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n))
elif i > x > y > n > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z))
elif i > x > z > y > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n))
elif i > x > z > n > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y))
elif i > x > n > y > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z))
elif i > x > n > z > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y))
elif i > y > x > z > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(n))
elif i > y > x > n > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(z))
elif i > y > z > x > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n))
elif i > y > z > n > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x))
elif i > y > n > x > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(n)+ ', ' +str(z))
elif i > y > n > z > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x))
elif i > z > x > y > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(n))
elif i > z > x > n > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(n)+ ', ' +str(y))
elif i > z > y > x > n:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(n))
elif i > z > y > n > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(n)+ ', ' +str(x))
elif i > z > n > x > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y))
elif i > z > n > y > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(z)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x))
elif i > n > x > y > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(y)+ ', ' +str(z))
elif i > n > x > z > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(x)+ ', ' +str(z)+ ', ' +str(y))
elif i > n > y > x > z:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(x)+ ', ' +str(z))
elif i > n > y > z > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(y)+ ', ' +str(z)+ ', ' +str(x))
elif i > n > z > x > y:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(x)+ ', ' +str(y))
elif i > n > z > y > x:
    print("El orden descendente es: " +str(i)+ ', ' +str(n)+ ', ' +str(z)+ ', ' +str(y)+ ', ' +str(x))


#La potencia del mayor numero elevado al menor numero
#Numero mayor
if x>y and x>z and x>n and x>i:
  numero_mayor = x
elif y>x and y>z and y>n and y>i:
  numero_mayor = y
elif z>x and z>y and z>n and z>i:
  numero_mayor = z
elif n>x and n>y and n>z and n>i:
  numero_mayor = n
elif i>x and i>y and i>z and i>n:
  numero_mayor = i
#Numero menor
if x<y and x<z and x<n and x<i:
  numero_menor = x
elif y<x and y<z and y<n and y<i:
  numero_menor = y
elif z<x and z<y and z<n and z<i:
  numero_menor = z
elif n<x and n<y and n<z and n<i:
  numero_menor = n
elif i<x and i<y and i<z and i<n:
  numero_menor = i
#Ecuación
resultado_potencia = (numero_mayor**numero_menor)
#Resultado
print("El resultado de la potencia es: "+str(resultado_potencia))


#La raiz cubica del menor numero
if x<=y and x<=z and x<=n and x<=i:
  x = float = x**(1/3)
  print("La raiz cubica es: "+str(x))
elif y<=x and y<=n and y<=z and y<=i:
  y = float = y**(1/3)
  print("La raiz cubica es: "+str(y))
elif z<=y and z<=i and z<=n and z<=x:
  z = float = z**(1/3)
  print("La raiz cubica es: "+str(z))
elif n<=y and n<=z and n<=x and n<=i:
  n = float = n**(1/3)
  print("La raiz cubica es: "+str(n))
elif i<=y and i<=x and i<=n and i<=z:
  i = float = i**(1/3)
#Resultado
  print("La raiz cubica es: "+str(i))
# 9.Escriba un programa que reciba el nombre en minúsculas de un país de America y retorne la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado.  
lang = input("Ingrese un país de America en minusculas ")

if lang == "argentina":
  print("Buenos Aires.")
elif lang ==  " canada":
  print("Otawwa. ")
elif lang ==  "estados unidos":
  print("Washington DC.")
elif lang ==  "mexico":
  print("México DF. ")
elif lang ==  "belice":
  print("Belmopán. ")
elif lang ==  "costa rica":
  print("San José. ")
elif lang ==  "salvador":
  print("San Salvador. ")
elif lang ==  "guatemala":
  print("Ciudad de Guatemala. ")
elif lang ==  "honduras":
  print("Tegucigalpa. ")
elif lang ==  "nicaragua":
  print("Managua. ")
elif lang ==  "panama":
  print("Panamá")
elif lang ==  "bolivia":
  print("Sucre ")
elif lang ==  "brasil":
  print("Brasilia ")
elif lang ==  "chile":
  print("Santiago ")
elif lang ==  "colombia":
  print("Bogotá ")
elif lang ==  "ecuador":
  print("Quito ")
elif lang ==  "paraguay":
  print("Asunción. ")
elif lang ==  "peru":
  print("Lima ")
elif lang ==  "surinam":
  print("Parabarimo. ")
elif lang ==  "uruguay":
  print("Montevideo ")
elif lang ==  "venezuela":
  print("Caracas")
elif lang ==  "antigua y barbuda":
  print("Saint John. ")
elif lang ==  "bahamas":
  print("Nasáu.")
elif lang ==  "barbados":
  print("Bridgetown.")
elif lang ==  "cuba":
  print("La Habana")
elif lang ==  "dominica":
  print("Roseau.")
elif lang ==  "granada":
  print("Saint George.")
elif lang ==  "guyana":
  print("Georgetown. ")
elif lang ==  "haiti":
  print("Puerto Príncipe. ")
elif lang ==  "jamaica":
  print("Kingston. ")
elif lang ==  "republica dominicana":
  print("Santo Domingo. ")
elif lang ==  "san cristóbal y nieves":
  print("Basseterre. ")
elif lang ==  "san vicente y las granadinas":
  print("Kingstown. ")
elif lang ==  "santa lucia":
  print("Castries. ")
elif lang ==  "chile":
  print("santiago. ")

else:
  print("Tu país no hace parte de America, recuerda escribirlo en minusculas.")
# Puntos pares
# 2.Realice un programa que lea tres números reales y determine cuál es el mayor.

a = float(input("Ingrese cualquier número: "))
b = float(input("Ingrese cualquier número: "))
c = float(input("Ingrese cualquier número: "))

if a > b and a > c:
    print(str(a) + " es el mayor")
elif b > a and b > c:
    print(str(b) + " es el mayor")
elif c > b and c > a:
    print(str(c) + " es el mayor")
elif a == b and a > c:
  print(str(a) + " es el mayor")
elif b == c and b > a:
  print(str(b) + " es el mayor")
elif a == c and a > b:
  print(str(a) + " es el mayor")
elif a == b and a == c:
  print("Todos son iguales")
# 4.Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.
a : float
b : float

a = float(input("Ingrese cualquier número: "))
b = float(input("Ingrese otro número: "))

if a % b == 0:
    print(str(a) + " es múltiplo de " + str(b))
else:
    print(str(a) + " no es múltiplo de " + str(b))
# 6.Escriba un programa que solicite al usuario una letra y determine si es una vocal o una consonante.

vocales = [65,69,73,79,85,97,101,105,111,117]
letra : str

letra = str(input("Ingrese cualquier letra: "))

if ord(letra) in vocales:
  print("Es una vocal")
else:
  print("Es una consonante")
# 8.Escriba un programa al que se le ingrese la frecuencia de una onda en hz y como salida arroje en que parte del espectro electromagnético se encuentra.

frecuencia_onda: float
frecuencia_onda = float(input("Ingrese la frecuencia de onda en hz: "))

if frecuencia_onda > 30.0*(10**18):
  print("rayos gamma")
elif frecuencia_onda	> 30.0*(10**15):
  print("Rayos X")
elif frecuencia_onda > 1.5*(10**15):
  print("ultravioleta extremo")
elif frecuencia_onda	> 7.89*(10**14):
  print("Ultravioleta cercano")
elif frecuencia_onda	 > 384*(10**12):
  print("Espectro Visible")
elif frecuencia_onda 	> 120*(10**12):
  print("Infrarrojo cercano	")
elif frecuencia_onda		> 6.00*(10**12):
  print("Infrarrojo medio")
elif frecuencia_onda > 300*(10**9):
  print("Infrarrojo lejano/submilimétrico")
elif frecuencia_onda > 3*(10**8):
  print("Microondas")
elif frecuencia_onda	> 300*(10**6):
  print("Ultra Alta Frecuencia-Radio")
elif frecuencia_onda	> 30*(10**6):
  print("Muy Alta Frecuencia-Radio")
elif frecuencia_onda	> 1.7*(10**6):
  print("Onda Corta - Radio")
elif frecuencia_onda	> 650*(10**3):
  print("Onda Media - Radio")
elif frecuencia_onda		> 30*(10**3):
  print("Onda Larga - Radio")
elif frecuencia_onda	< 30*(10**3):
  print("Muy Baja Frecuencia - Radio")
# 10.Escriba un programa que dada una distancia calcule:

#El tiempo que le tomaría a la luz recorrer la distancia.
#El tiempo que le tomaría al sonido (en el aire) recorrer la distancia.
#El tiempo que le tomaría al vehiculo comercial más veloz recorrer la distancia.
#El tiempo que le tomaría a Bolt recorrer la distancia.

distancia : float
distancia = float(input("Ingrese una distancia en m/s: "))
print("A la luz le tomaría " + str(distancia/299792458) + " segundos recorrer esa distancia")
print("Al sonido le tomaría " + str(distancia/343) + " segundos recorrer esa distancia")
print("Al vehiculo comercial más veloz le tomaría " + str(distancia/126.9 ) + " segundos recorrer esa distancia")
print("A Bolt le tomaría " + str(distancia/12.27 ) + " segundos recorrer esa distancia")

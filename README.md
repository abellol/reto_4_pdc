# reto_4_pdc
### La solución está en el archivo reto_4.ipynb, sin embargo acá los codigos individuales
#### Ejercicio 1
```python
print("Escriba un número positivo:")
num = input()

try:
    a = int(num)
    b = chr(a)
    print(b)

    match b:
        case "a":
            print("El código", a, "pertenece a la vocal a del código ASCII")
        case "e":
            print("El código", a, "pertenece a la vocal e del código ASCII")
        case "i":
            print("El código", a, "pertenece a la vocal i del código ASCII")
        case "o":
            print("El código", a, "pertenece a la vocal o del código ASCII")
        case "u":
            print("El código", a, "pertenece a la vocal u del código ASCII")
        case _:
            print("El código", a, "no pertenece a ninguna vocal del código ASCII")

except ValueError:
    print("No es un número positivo")
```
#### Ejercicio 2
```python
print("escriba un (1) caracter:")
txt = input()
try: 
    len(txt) == 1
    b=ord(txt)
    print(b)
    x=str(b)
    y=int(x[0])
    
    if y % 2 == 0:
        print("El primer digito del codigo ASCII del caracter", txt, "es par")
    else:
        print("El primer digito del codigo ASCII del caracter", txt, "no es par")
except TypeError:
    print("no es un (1) caracter")

```
#### Ejercicio 3
```python
print("Escriba una cadena caracteres")
c = input()

len(c) == 1
if c.isalpha() ==True:
    print("Su caracter", c, "no es un digito")
elif c.isdigit() == True:
    print("Su caracter", c, "es un digito")
else:
    print("su caracter",c, "no es un digito")
```
#### Ejercicio 4
```python
print("Escriba un numero real:")
x = input()
try:
    x=float(x)
    if x > 0:
        print("El número",x, "es positivo")
    elif x < 0:
        print("El número", x, "es negativo")
    elif x == 0:
        print ("El número", x, "es el neutro para la suma")
except ValueError:
    print("el caracter", x, "no es un numero real")
```
#### Ejercicio 5
```python
centro1 : float
centro2 : float
radio : float
punto1 : float
punto2 : float
try:
    centro1 = float(input("Ingrese la coordenada x para el centro del circulo: "))
    centro2 = float(input("Ingrese la coordenada y para el centro del circulo: "))
    radio = float(input("Ingrese el radio del circulo: "))
    punto1 = float(input("Ingrese la coordenada x del punto a verificar: "))
    punto2 = float(input("Ingrese la coordenada y del punto a verificar: "))
   
    if (punto1 - centro1)**2 + (punto2- centro2)** 2<= radio**2:
        print("La coordenada ingresada (" ,punto1, " , " ,punto2, ") se encuentra dentro del circulo formado por el centro (" ,centro1, " , " ,centro2, ") con radio " ,radio)
    else:
        print("La coordenada ingresada (" ,punto1, " , " ,punto2, ") no se encuentra dentro del circulo formado por el centro (" ,centro1, " , " ,centro2, ") con radio " ,radio)
except ValueError:
    print("El valor ingresado no es un numero real")
```
#### Ejercicio 6
```python
long1 = (input ("Escriba la primera longitud positiva:", ))
long2 = (input ("Escriba la segunda longitud positiva:", ))
long3 = (input ("Escriba la tercera longitud positiva:", ))
t = "Las medidas no pueden formar un triangulo"
try:
    a= abs(float(long1))
    b= abs(float(long2))
    c= abs(float(long3))
    print(a)
    print(b)
    print(c)
    if a + b < c:
        print (t)
    elif b + c < a:
        print(t)
    elif a + c < b:
        print(t)
    else:
        print("las medidas si pueden formar un triangulo")
except ValueError:
    print("alguna dimension no es un numero")
```


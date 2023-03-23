# Reto-5 

1. En este caso se declara una variable entera que corresponderá al el número en cuestión. El valor que se establece es comparado con cada uno de los números equivalentes a las vocales minúsculas; si tienen relación de igualdad se envia el mensaje: "El número " + str(numero) + " corresponde una vocal minúscula en código ASCCI", de lo contrario se envía "El número "+ str(numero) + " no corresponde a una vocal minúscula en código ASCCI":

Código:

```
#Programa para determinar si un número entero corresponde a una vocal minúscula en código ASCCI.
numero: int 
numero = int(input("Introducir número entero"))

if numero == 97 or numero == 101 or numero == 105 or numero == 111 or numero == 117:
    print("El número " + str(numero) + " corresponde una vocal minúscula en código ASCCI")
else:
    print("El número "+ str(numero) + " no corresponde a una vocal minúscula en código ASCCI")
``` 
En acción para numero = 112: 

[![2023-03-22-1.png](https://i.postimg.cc/x8mRns4w/2023-03-22-1.png)](https://postimg.cc/bSzbRR8g)

2. En primer lugar se introduce la cadena de longitud 1; luego se utiliza la función ord() para llevarla a código ASCCI. Posteriormente se evalúa el módulo del resultado entre dos. Si es distinto de cero se imprime un mensaje afirmando que "El código ASCII de primera letra de la cadena es impar", de lo contrario el módulo es igual a cero y el programa imprime "El código ASCII de primera letra de la cadena es par".

Código:

```
#Programa que dada una cadena de longitud 1, determina si el código ASCII de primera letra de la cadena es par o no.

cadena = input("Cadena de longitud 1")

if ord(cadena)%2 != 0:
    print("El código ASCII de primera letra de la cadena es impar")
else:
    print("El código ASCII de primera letra de la cadena es par") 
```
En acción para cadena = "a":

[![2023-03-22-2.png](https://i.postimg.cc/YqwVjgz6/2023-03-22-2.png)](https://postimg.cc/w30FG1PM)

[![2023-03-22-3.png](https://i.postimg.cc/pXYSjTsg/2023-03-22-3.png)](https://postimg.cc/w7MF868V)

3. En este caso se utiliza la función isdigit() para determinar si el caracter que se solicita ingresar al inicio del programa correspponde a un número. Si la función arroja True, el caracter corresponde a un número y se imprime este mensaje, si arrojara False se imprime un mensaje confirmando que el caracter ingresado no corresponde a un número.

Código:
```
#Programa que dado un caracter x, determina si el carácter es un dígito o no.

caracter = input("Insertar caracter")

if caracter.isdigit() == True:
    print("El caracter ingresado es un número.")
else:
     print("El caracter ingresado no es un número.")
```

En acción para 89 y attack:

[![2023-03-22-4.png](https://i.postimg.cc/SxmxLnk8/2023-03-22-4.png)](https://postimg.cc/JGd8M4y4)

[![2023-03-22-5.png](https://i.postimg.cc/0NQ53h6y/2023-03-22-5.png)](https://postimg.cc/DS9K4jd9)

[![2023-03-22-6.png](https://i.postimg.cc/MGFZ8tRb/2023-03-22-6.png)](https://postimg.cc/5H8WBBs6)

[![2023-03-22-7.png](https://i.postimg.cc/7ZXYKqZR/2023-03-22-7.png)](https://postimg.cc/NK9cMqT8)

5. Para el problema 5 primeramente se declaran y se le asigna un valor a las variables correspoondientes a las coordenadas del centro del círculo, el punto R2 y el valor del radio. Luego para calcular si R2 se encuentra dentro de la circunferencia debe de rpobarse que la distancia entre el punto y el centro es igual o menor al radio. Para ello se emplea el teorema de Pitágorás. 
 Código:
 ```
 #Programa que, dado el centro y el radio de un círculo, determina si un punto de R2 pertenece o no al interior del círculo.
centrox: float
centroy: float
R2x: float
R2y: float
radio: float

centrox = float(input("Insertar valor de la coordenada  x del centro del círculo"))
centroy = float(input("Insertar valor de la coordenada y del centro del círculo"))
R2x = float(input("Insertar valor de la coorenada x del punto R2"))
R2y = float(input("Insertar valor de la coordenada y del punto R2"))
radio = float(input("Insertar valor del radio del círculo"))

if radio >= ((R2x - centrox)**2 + (R2y - centroy)**2)**0.5:
    print("El punto " + str(R2x) + "," + str(R2y) + " pertenece al circulo de centro " + str(centrox) + ", " + str(centroy) + " y radio " + str(radio))
else:
    print("El punto " + str(R2x) + "," + str(R2y) + " no pertenece al circulo de centro " + str(centrox) + ", " + str(centroy) + " y radio " + str(radio))
```
    
En acción  para Pto R2 = (0,3) Radio = 10 y centro = (0,0): 

[![2023-03-22-8.png](https://i.postimg.cc/sXt68VCz/2023-03-22-8.png)](https://postimg.cc/R6LLJx0p)

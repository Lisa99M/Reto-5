#Reto 5#

'''
#Programa para determinar si un número entero corresponde a una vocal minúscula en código ASCCI.
numero: int 
numero = int(input("Introducir número entero"))

if numero == 97 or numero == 101 or numero == 105 or numero == 111 or numero == 117:
    print("El número " + str(numero) + " corresponde una vocal minúscula en código ASCCI")
else:
    print("El número "+ str(numero) + " no corresponde a una vocal minúscula en código ASCCI")
'''

'''#Programa que dada una cadena de longitud 1, determina si el código ASCII de primera letra de la cadena es par o no.

cadena = input("Cadena de longitud 1")

if ord(cadena)%2 != 0:
    print("El código ASCII de primera letra de la cadena es impar")
else:
    print("El código ASCII de primera letra de la cadena es par") 
'''

'''
#Programa que dado un caracter x, determina si el carácter es un dígito o no.

caracter = input("Insertar caracter")

if caracter.isdigit() == True:
    print("El caracter ingresado es un número.")
else:
     print("El caracter ingresado no es un número.")
     '''

     '''
     #Programa que dado un numero real x, permite determinar si el número es positivo, negativo o cero.

x: float
x = float(input("Insertar valor de x"))

if x < 0:
    print("El numero " + str(x) + " es negativo.")
elif x > 0:
    print("El numero " + str(x) + " es positivo.")
else:
    print("El número " + str(x) + " es el neutro para la suma")
 '''

 '''
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
    '''
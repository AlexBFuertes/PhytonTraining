# PhytonTraining
import sys
print(sys.version)
print("Hello world")
####################################################
if 1 > 2:
  print("Five is greater than two!")
else:
  print("Nope")
####################################################
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
print(x, y, z)
####################################################
def myfunc():
  print("Python is " + x)
####################################################
myfunc()
a = "Hello, World!"
print(a[7])
print(a[2:5]) #preguntar qué quiere decir este código
print(a[-5:-2]) #Los últimos cinco y dos caracteres
print(len(a)) #Longitud de la cadena
print(a.lower()) #Cadena en minúsculas
print(a.upper()) #Cadena en mayúsculas
print(a.replace("H", "J")) #Reemplazar caracteres
print(a.split(",")) #Dividir cadena
print("Enter your name:") #Imprimir mensaje
####################################################
for x in "banana":
  print(x) #Imprimir cada letra de la cadena
####################################################
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, 'free' is present.") #Buscar una palabra en la cadena
####################################################
txt = "The best things in life are expensive!"
print("expensive" not in txt) #Buscar una palabra en la cadena
####################################################
b = "Hello, World!"
print(b[:5]) #Imprimir los primeros cinco caracteres
print(b[2:]) #A partir del tercer caracter
####################################################
a = " Hello, World! "
print(a.strip()) # returns "Hello, World!"
####################################################
a = "Hello"
b = "World"
c = a + b
print(c) #imprime "HelloWorld"
####################################################
a = "Hello"
b = "World"
c = a + " " + b
print(c) #Imprime "Hello World"
####################################################
age = 36
txt = f"My name is John, I am {age}" #Se debe poner "f" para que funcione
print(txt) #My name is John, I am 36
####################################################
price = 59
txt = f"The price is {price:.2f} dollars" #Con ":.2f" añade dos ceros tras un punto
print(txt) #The price is 59.00 dollars
####################################################
txt = "Hello\nWorld!"
print(txt) #Hello
           #World
####################################################
class myclass():
  def __len__(self):
    return 0 #myclass vale y devuelve el número de aquí
####################################################
myobj = myclass()
print(bool(myobj)) #El valor de myobj es el que devuelve myclass porque myclass=myobj

def myFunction() :
  return False #myFunction devuelve su valor (True o False)

if myFunction():
  print("YES!") #Si myFunction es True
else:
  print("NO!") #Si myFuction es false
####################################################
x = 200
print(isinstance(x, int)) #"insistance" para determinar si es verdadero o falso
####################################################
thislist = ["apple", "banana", "cherry"]
print(thislist)
####################################################
thislist = ["apple", "banana", "cherry"]
print(thislist[1]) #Para determinar cuál deseamos en la salida
####################################################
thislist = ["apple", "banana", "cherry"]
print(thislist[-1]) #Vuelve por el último empezando el print por cherry
####################################################
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])
####################################################
#This will return the items from position 2 to 5.

#Remember that the first item is position 0,
#and note that the item in position 5 is NOT included

thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")
####################################################
thislist = ["apple", "banana", "cherry"]
thislist[1] = "blackcurrant" #Se sustituye posición 1 con la palabra de la derecha

print(thislist) #apple, blackcurrant, cherry
####################################################
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]

thislist[1:3] = ["blackcurrant", "watermelon"]

print(thislist) #['apple', 'blackcurrant', 'watermelon', 'orange', 'kiwi', 'mango']
####################################################
thislist = ["apple", "banana", "cherry"]

thislist.insert(2, "watermelon")

print(thislist) #["apple", "banana", "watermelon", "cherry"]
####################################################
thislist = ["apple", "banana", "cherry"]

thislist.append("orange")

print(thislist) #['apple', 'banana', 'cherry', 'orange']
####################################################
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]

thislist.extend(tropical)

print(thislist) #['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya']
####################################################
thislist = ["apple", "banana", "cherry"]
thislist.remove("banana") #Para borrar elementos
print(thislist)
####################################################
thislist = ["apple", "banana", "cherry"]
thislist.pop(1) #Para remover posición
print(thislist)
####################################################
thislist = ["apple", "banana", "cherry"]
thislist.pop() #Sin especificar borra el último elemento
print(thislist) #["apple", "banana"]
####################################################
thislist = ["apple", "banana", "cherry"]
del thislist #Borra todo
####################################################
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist) #"[]"
####################################################
thislist = ["apple", "banana", "cherry"]
for x in thislist:
  print(x)
### "apple
### banana
### cherry"
####################################################
thislist = ["apple", "banana", "cherry"]
i = 0
while i < len(thislist):
  print(thislist[i])
  i = i + 1 #Cuando i=0; nombra los tres. Cuando i=1; nombre banana y cherry y
  #cuando i=2; nombra cherry tan solo.
####################################################
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)
#Se nombran sólo las frutas con la letra "a".
print(newlist)
####################################################
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = [x for x in fruits if not "a" in x]

print(newlist) #['cherry', 'kiwi']
####################################################
newlist = [x for x in range(10)]

print(newlist) #[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
####################################################
newlist = [x for x in range(10) if x < 5]

print(newlist) #[0, 1, 2, 3, 4]
####################################################
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x.upper() for x in fruits]

print(newlist) #['APPLE', 'BANANA', 'CHERRY', 'KIWI', 'MANGO']
####################################################
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = ['hello' for x in fruits]

print(newlist) #['hello', 'hello', 'hello', 'hello', 'hello']
####################################################
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x if x != "banana" else "orange" for x in fruits]

print(newlist) #['apple', 'orange', 'cherry', 'kiwi', 'mango']
####################################################
'''
OPERACIONES ARITMÉTICAS
+ SUMA
- RESTA
* MULTIPLICACIÓN
/ DIVISIÓN
// DIVISIÓN ENTERA
% MÓDULO
** POTENCIA
exercism NOMBRE DE PÁGINA WEB PARA PRÁCTICAR PROGRAMACIÓN
'''

n1 = 4
n2 = 4
r = 4 + 4
print(r)
####################################################
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]

thislist.sort() #Ordena alfabéticamente o de menor a mayor (números)

print(thislist)
####################################################
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]

thislist.sort(reverse = True) #Empezar por banana y acabar por orange

print(thislist)
####################################################
thislist = [100, 50, 65, 82, 23]

thislist.sort(reverse = True) #De mayor a menor

print(thislist)
####################################################
def myfunc(n):
  return abs(n - 50) #Return la resta de los elementos

thislist = [100, 50, 65, 82, 23]

thislist.sort(key = myfunc) #Ordenar de mayor a menor el valor resultante de la resta

print(thislist) #[50, 65, 23, 82, 100]
####################################################

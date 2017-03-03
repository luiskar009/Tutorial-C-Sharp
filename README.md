# Tutorial-C-Sharp
Instrucciones c#
#Operaciones con Strings
* Concatenar dos Strings
```[csharp]
String concat = "HOLA + "MUNDO";
```
* Convertir el String a mayusculas
```[csharp]
String a = "hola";
a = a.ToUpper(); //a contendria "HOLA"
```
* Convertir el String a minusculas
```[csharp]
String a = "HOLA";
a = a.ToLower(); //a contendria "hola"
```
* Eliminar espacios de un String
```[csharp]
String a = "Hola Mundo";
a = a.Trim(); //a contendria "HolaMundo"

String b = "  Hola Mundo"; 
b = b.TrimStart(); //b contrendria "Hola Mundo"

String c = "Hola Mundo  "
c = c.TrimEnd(); //c contedria "Hola Mundo"
```
* Eliminar parte de un String
```[csharp]
String a = "Hola Mundo";
a = a.SubString(0,5); // SubString(inicio,final) recorta el string desde la posicion inical 
                      // a la final, por lo que a contendria "Hola M"
```
* Introducir una variable a un string
```[csharp]
int i = 5
String a = String.Format("Pedro tiene {0} coches, i);" //Introduce en {0} el valor guardado en i
```
* Remplazar una parte del string por otra
```[csharp]
String a = Hola Mundo"
a = String.Replace("Mundo","Nuevo"); //Introduce en Cambia Mundo por Nuevo
```
* Saber si un string contiene un substring
```[csharp]
String a = "Hello World";
bool b = a.Contains("Hello"); // b contendria true
```

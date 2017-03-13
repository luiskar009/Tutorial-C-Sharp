# Tutorial-C-Sharp
Instrucciones c#
## Indice

1. [Operaciones con Strings](#operaciones-con-strings)
2. [Operaciones con DateTime](#operaciones-con-datetime)

## Operaciones con Strings
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
## Operaciones con DateTime
* Mostrar la fecha y la hora en este momento
```[csharp]
DateTime a = DateTime.Now(); 
```
* Mostrar la fecha de hoy
```[csharp]
DateTime a = DateTime.Today(); 
```
* Constructor DateTime nuevo
```[csharp]
DateTime a = new DateTime(2017,8,1); //Unicamente la fecha (año,mes,dia)
DateTime b = new DateTime(2017,8,1,8,0,0); // Fecha y hora (año,mes,dia,hora,minuto,segundo)
```
* Modificar una fecha guardada
```[csharp]
DateTime a = DateTime.Now(); 
DateTime b = a.AddYear(1); // Añade o quita años, dependiendo de si el valor es pòsitivo o negativo
DateTime c = a.AddMonths(1); // Añade o quita meses, dependiendo de si el valor es pòsitivo o negativo
DateTime d = a.AddDays(1); // Añade o quita dias, dependiendo de si el valor es pòsitivo o negativo
DateTime e = a.AddHours(1); // Añade o quita horas, dependiendo de si el valor es pòsitivo o negativo
DateTime f = a.AddMinutes(1); // Añade o quita minutos, dependiendo de si el valor es pòsitivo o negativo
DateTime g = a.AddSeconds(1); // Añade o quita segundos, dependiendo de si el valor es pòsitivo o negativo
```
* Pasar un String a DataTime
```[csharp]
String a = "01-01-2017";
DateTime b = DateTime.Parse(a); 
```
* Devolver una parte de una fecha DateTime
```[csharp]
DateTime a = DateTime.Now();
int b = a.Year // Devuelve el año de la fecha
int c = a.Month // Devuelve el año de la fecha
int d = a.Day // Devuelve el año de la fecha
int e = a.Hour // Devuelve el año de la fecha
int f = a.Minute // Devuelve el año de la fecha
int g = a.Second // Devuelve el año de la fecha
```
* Operaciones con fechas
La fechas se pueden sumar o restar utilizando los operandos (+,-).


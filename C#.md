# C Sharp
## Indice
1. [Operaciones con Strings](#operaciones-con-strings)
2. [Operaciones con DateTime](#operaciones-con-datetime)
3. [Arrays](#arrays)
4. [Listas](#listas)
## Operaciones con Strings
* Concatenar dos Strings
```csharp
string concat = "HOLA" + "MUNDO";
```
* Convertir el String a mayusculas
```csharp
string a = "hola";
a = a.ToUpper(); //a contendria "HOLA"
```
* Convertir el String a minusculas
```csharp
string a = "HOLA";
a = a.ToLower(); //a contendria "hola"
```
* Eliminar espacios de un String
```csharp
string a = "Hola Mundo";
a = a.Trim(); //a contendria "HolaMundo"

string b = "  Hola Mundo"; 
b = b.TrimStart(); //b contrendria "Hola Mundo"

string c = "Hola Mundo  "
c = c.TrimEnd(); //c contedria "Hola Mundo"
```
* Eliminar parte de un String
```csharp
string a = "Hola Mundo";
a = a.SubString(0,5); // SubString(inicio,final) recorta el string desde la posicion inical 
                      // a la final, por lo que a contendria "Hola M"
```
* Introducir una variable a un string
```csharp
int i = 5
string a = String.Format("Pedro tiene {0} coches", i); //Introduce en {0} el valor guardado en i
```
* Remplazar una parte del string por otra
```csharp
string a = "Hola Mundo"
a = String.Replace("Mundo","Nuevo"); //Introduce en Cambia Mundo por Nuevo
```
* Saber si un string contiene un substring
```csharp
string a = "Hola Mundo";
bool b = a.Contains("Hola"); // b contendria true
```
* Saber si un string empieza o termina en un string
```csharp
string a = "Hola Mundo";
bool b = a.StartsWith("Hola"); // b contendria true
bool b = a.EndsWith("Mundo"); // b contendria true
```
## Operaciones con DateTime
* Mostrar la fecha y la hora en este momento
```csharp
DateTime a = DateTime.Now(); 
```
* Mostrar la fecha de hoy
```csharp
DateTime a = DateTime.Today(); 
```
* Constructor DateTime nuevo
```csharp
DateTime a = new DateTime(2017,8,1); //Unicamente la fecha (año,mes,dia)
DateTime b = new DateTime(2017,8,1,8,0,0); // Fecha y hora (año,mes,dia,hora,minuto,segundo)
```
* Modificar una fecha guardada
```csharp
DateTime a = DateTime.Now(); 
DateTime b = a.AddYear(1); // Añade o quita años, dependiendo de si el valor es pòsitivo o negativo
DateTime c = a.AddMonths(1); // Añade o quita meses, dependiendo de si el valor es pòsitivo o negativo
DateTime d = a.AddDays(1); // Añade o quita dias, dependiendo de si el valor es pòsitivo o negativo
DateTime e = a.AddHours(1); // Añade o quita horas, dependiendo de si el valor es pòsitivo o negativo
DateTime f = a.AddMinutes(1); // Añade o quita minutos, dependiendo de si el valor es pòsitivo o negativo
DateTime g = a.AddSeconds(1); // Añade o quita segundos, dependiendo de si el valor es pòsitivo o negativo
```
* Pasar un String a DataTime
```csharp
string a = "01-01-2017";
DateTime b = DateTime.Parse(a); 
```
* Devolver una parte de una fecha DateTime
```csharp
DateTime a = DateTime.Now();
int b = a.Year; // Devuelve el año de la fecha
int c = a.Month; // Devuelve el año de la fecha
int d = a.Day; // Devuelve el año de la fecha
int e = a.Hour; // Devuelve el año de la fecha
int f = a.Minute; // Devuelve el año de la fecha
int g = a.Second; // Devuelve el año de la fecha
```
* Operaciones con fechas
La fechas se pueden sumar o restar utilizando los operandos (+,-).

## Arrays

* Constructor array
```csharp
int[] a = new int[5]; //Crea un array de tipo int con 5 elementos vacios
int[] b = new int[5]{1,2,3,4,5}; //Crea un array de tipo int con 5 elementos y lo rellena
string[][] c = new string [][]; //Crea un array matriz
```
* Concatenar elementos de un array en un string
```csharp
int[] a = new int[2]{0,1};
string b = string.Join("-",a); //b contiene la cadena "0-1"
```
* Crear array a partir de una cadena de strings
```csharp
string a = "a/b/c";
string[] b = new string[3];
b = Regex.Split(a,"/"); // Guardaria a en la posicion 0, b en la posicion 1 y c en la posicion 2
```
* Saber el tamaño de un array
```csharp
int[] a = new int[2];
int b = a.Length; // Devolveria 2
```
* Pasar un elemento del array a string
```csharp
int[] a = new int[2]{0,1};
string b = a[0].ToString(); //b contendria "0"
```
* Recorrer un array
```csharp
int[] a = new int[2]{0,1};
foreach (int element in a)
{
//aqui se haria lo que se quisiera con cada elemento
}
```
## Listas
* Constructor lista
```csharp
List<string> list = new List<string>();
```
* Añadir elemento a la lista
```csharp
list.Add("a"); //Añade "a" a list
```
* Borrar un elemento de la lista
```csharp
list.Remove("a"); //Elimina "a" a list
```
* Insertar un elemento a la lista
```csharp
list.Remove(2, "a"); //Añade "a" a list en la posicion 2
```
* Eliminar elementos de una lista que cumplan una condicion
```csharp
list.RemoveAll(string.ToLower().EndsWith("br")); //Elimina todos los elementos terminados en br
```
* Eliminar elemento por posicion
```csharp
list.RemoveAt(2); //Elimina el elemento colocado en la posicion 2
```
* Vaciar la lista
```csharp
list.Clear(); //Deja la lista vacia de elementos
```
* Saber el numero de elementos que contiene una lista
```csharp
int a = list.Count(); //Devuelve el numero de elementos
```
* Recorrer lista
```csharp
foreach(int element in list)
{
//aqui se haria lo que se quisiera con cada elemento
}
```


# Tutorial-C-Sharp
Instrucciones c#
## Indice

1. [Conexion a Base de Datos](#conexion-a-base-de-datos)

## Conexion a Base de Datos

* String de conexion
```csharp
string connString = "Data Source=myServerAddress; Initial Catalog=myDataBase; Integrated Security=True; 
user id = user; password = pass;"
```
Data Source -> Identifica el servidor. Puede ser una maquina local, un dominio o una direccion IP    
Initial Catalog -> La base de datos que abrira esa conexion por defecto  
User id -> Usuario de la BD  
Password -> Contraseña de la BD  

* Crear la variable de conexion

```csharp
SqlConnection conn = new SqlConnection(connString);
```

* Abrir una conexion

```csharp
conn.Open();
```

* Cerrar una conexion

```csharp
conn.Close();
```

* Cambiar la BD de una conexion 

```csharp
conn.ChangeDatabase("nombreBD");
```

* Cerrar la Base de Datos automaticamente cuando se termina de trabajar con ella

```csharp
using (SqlConnection conn = new SqlConnection(connString))
{
//Aqui iria todas las operaciones que se harian con la base de datos
}
```

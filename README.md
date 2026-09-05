# Proyecto: Análisis de Datos Hospitalarios con SQL y Python 🏥
Pequeño proyecto sobre el análisis de datos de una base de datos hospitalaria mediante SQL, Pandas, Matplotlib y Seaborn.

## ¿Qué pretende este proyecto?
En este caso he buscado integrar el uso de SQL a mis conocimientos previos sobre Big Data, realizando consultas sobre una base de datos PostgreSQL y utilizando posteriormente librerías de Data Science
para analizar y visualizar los resultados.

## Resumen del proyecto
En este proyecto empleo una base de datos ficticia de un hospital, con información acerca de pacientes, médicos, citas, medicamentos, recetas, ingresos y salas hospitalarias. Primeramente realizo la conexión con la 
base de datos Hospital, mediante la función `create_engine()`, donde debemos indicar el nombre de usuario, nuestra contraseña, el host, el puerto y el nombre de la bbdd.

Una vez establecida la conexión, planteo una serie de consultas para trabajar con SQL e integrarlo con Python. Algunas de estas consultan son:
- ¿Cuál es el medicamento más recetado a los pacientes?
- ¿Qué especialidades tienen una mayor demanda de citas?
- ¿Qué salas de hospital han tenido más ingresos?
- ¿Qué pacientes han estado ingresados más de una vez por arritmia?

En estas consultas hago uso de `INNER JOIN, LEFT JOIN, WHERE, GROUP BY, ORDER BY, HAVING, CASE, COUNT(), LIMIT`, así como de una CTE con `WITH ... AS`

Una vez obtenidos los resultados, utilizo Pandas para cargar los datos en un DataFrame, y posteriormente empleo Matplotlib y Seaborn para representar gráficamente los resultados, utilizando mayormente el gráfico `barplot`


## Para ejecutar el script...
Se necesita tener un intérprete de Python que contenga las librerías SQLAlchemy, Pandas, Matplotlib y Seaborn. En mi caso utilizo conda (obtenible mediante la descarga de Anaconda), por lo que solo he tenido que 
instalar SQLAlchemy `pip install sqlalchemy`

En mi caso, al trabajar con PostgreSQL, he tenido que instalar el driver de comunicación con la base de datos: `pip install psycopg2-binary`

El proyecto está desarrollado en formato `.ipynb`, por lo que se necesita la extensión de Jupyter para poder visualizarlo y ejecutarlo desde VS Code.

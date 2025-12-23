///Descripción del proyecto

Aplicación desarrollada por Gabriel Primera Ceballos en el marco del programa Oracle Next Education (ONE).

El proyecto consiste en una aplicación Java basada en Spring Boot que consume la API pública Gutendex para obtener información de libros y almacenarla en una base de datos local.
Permite realizar búsquedas, registrar información y consultar libros a través de un menú interactivo por consola, utilizando Spring Data JPA para la persistencia de datos.

Este desarrollo forma parte de los desafíos finales del programa ONE – Oracle Next Education.

//Funcionalidades

La aplicación permite realizar las siguientes operaciones desde la consola:
Consultar libros desde la API Gutendex y guardarlos en la base de datos
Buscar libros por nombre de autor
Buscar libros por título
Visualizar los 10 libros con mayor cantidad de descargas
Obtener la cantidad de libros disponibles en español e inglés
Listar autores que se encontraban vivos en un año específico

//Tecnologías y herramientas utilizadas:

- Java 17
- Spring Boot
- Spring Data JPA
- Hibernate
- H2 Database
- Jackson (procesamiento JSON)
- Maven

//Base de datos
- La base de datos se genera automáticamente al iniciar la aplicación
- No requiere configuración previa por parte del usuario
- Las tablas se crean a partir de las entidades definidas con JPA

///El Proyecto.

src/main/java
└── com.catalogo.literatura
    ├── config
    ├── modelo
    │   ├── Autor.java
    │   └── Libro.java
    ├── principal
    │   ├── ClienteGutendex.java
    │   ├── DatosAutor.java
    │   ├── DatosGutendex.java
    │   ├── DatosLibro.java
    │   └── MenuConsola.java
    ├── repositorio
    │   └── RepositorioLibros.java
    └── CatalogoLiteraturaApplication.java

src/main/resources
└── application.properties

// Cómo ejecutar el proyecto

1. Clonar el repositorio desde GitHub
2. Abrir el proyecto en un IDE como IntelliJ IDEA o Eclipse
3. Ejecutar la aplicación como proyecto Spring Boot
4. Utilizar el menú en consola para interactuar con el sistema

//Vista del catalogo

===== CATÁLOGO DE LITERATURA =====
1 - Buscar libros desde la API
2 - Buscar libros por autor
3 - Buscar libros por título
4 - Top 10 libros más descargados
5 - Cantidad de libros en español e inglés
6 - Listar autores vivos en un año
0 - Salir

//API utilizada

Gutendex API
API pública basada en el proyecto Gutenberg
https://gutendex.com/



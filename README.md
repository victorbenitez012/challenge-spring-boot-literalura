# LiterAlura

**LiterAlura** es una aplicación de consola desarrollada en Java utilizando Spring Boot, diseñada para gestionar una biblioteca personal de libros y autores. La aplicación interactúa con la API de Gutendex para obtener información sobre libros y autores, almacenándola en una base de datos local para su posterior consulta.

## Características

- **Búsqueda de libros por título**: Permite al usuario buscar libros por su título.
- **Listado de libros registrados**: Muestra todos los libros almacenados en la base de datos.
- **Listado de autores registrados**: Muestra todos los autores de libros almacenados en la base de datos.
- **Listado de autores vivos en un año específico**: Permite al usuario ingresar un año y muestra todos los autores que estaban vivos en ese año, basándose en la información de los libros almacenados.
- **Listado de libros por idioma**: Permite al usuario ingresar un idioma y muestra todos los libros disponibles en ese idioma, utilizando la información de la API de Gutendex y la base de datos.
- **Top 10 de libros más descargados**: Muestra los 10 libros más descargados almacenados en la base de datos.
- **Estadísticas de descargas**: Proporciona estadísticas sobre las descargas de libros, incluyendo total, promedio, mínimo y máximo.

## Tecnologías Utilizadas

- **Java 17**: Lenguaje de programación principal.
- **Spring Boot 3.2**: Framework para el desarrollo de aplicaciones Java.
- **Spring Data JPA**: Para la interacción con la base de datos.
- **PostgreSQL**: Sistema de gestión de bases de datos.
- **Gutendex API**: API externa para obtener información sobre libros y autores.

## Instalación

1. **Clonar el repositorio**:

   ```bash
   git clone https://github.com/victorbenitez012/challenge-spring-boot-literalura.git
   cd challenge-spring-boot-literalura
Configurar la base de datos:

Asegúrate de tener PostgreSQL instalado y en funcionamiento. Crea una base de datos llamada literAlura y configura las credenciales en el archivo src/main/resources/application.properties:

properties
Copiar
Editar
spring.datasource.url=jdbc:postgresql://localhost:5432/literAlura
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
Ejecutar la aplicación:

Puedes ejecutar la aplicación desde tu IDE favorito o utilizando Maven desde la línea de comandos:

bash
Copiar
Editar
mvn spring-boot:run
Uso
Al iniciar la aplicación, se presentará un menú en la consola con las siguientes opciones:

css
Copiar
Editar
[1] - Buscar Libro por Titulo
[2] - Listar Libros Registrados
[3] - Listar Autores Registrados
[4] - Listar Autores vivos en un determinado año
[5] - Listar Libros por Idioma
[6] - Buscar Autor por nombre
[7] - Listar Autores por rango de años de Nacimiento
[8] - Top 10 Libros más descargados
[9] - Estadísticas
[0] - Salir
Selecciona la opción deseada ingresando el número correspondiente y sigue las instrucciones en pantalla.

Estructura del Proyecto
src/main/java/com/jonatan/literAlura: Contiene el código fuente de la aplicación.
principal: Contiene la clase Principal, que gestiona la ejecución de la aplicación.
model: Contiene las clases de modelo (Libro, Autor, LibroDTO, AutorDTO).
repository: Contiene las interfaces de repositorio Spring Data JPA.
service: Contiene las clases de servicio (ConsumoApi, ConvierteDatos).
src/main/resources: Contiene los archivos de configuración de la aplicación.
pom.xml: Contiene las dependencias del proyecto.
Contribuciones
Las contribuciones son bienvenidas. Si tienes sugerencias, correcciones de errores o mejoras, siéntete libre de abrir un issue o enviar un pull request.

Licencia
Este proyecto está licenciado bajo la Licencia MIT.

Autor
Este proyecto fue desarrollado por Víctor Benítez.

Agradecimientos
Gracias a Gutendex por proporcionar la valiosa información sobre libros y autores.
Gracias a la comunidad de Spring Boot por el robusto framework.
php
Copiar
Editar

Este archivo README proporciona una visión clara y detallada de tu proyecto, incluyendo sus características, tecnologías utilizadas, instrucciones de instalación y uso, estructura del proyecto, y cómo contribuir.
::contentReference[oaicite:0]{index=0}
by insider
 

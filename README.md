# Trabajo Práctico JPA
Proyecto donde se realiza auditoría de las entidades persistidas en el ejemplo del [repositorio de JPA](https://github.com/jpbiondo/trabajo-practico-jpa/) con Envers en Hibernate.

## Estructura del proyecto
El paquete `org.example.entidades` contiene todas las clases de las entidades a persistir. En el paquete de `org.example.audit` se encuentra la entidad del registro de auditoría a persistir y en el paquete `org.example.config` el listener a las creación de registros de auditoría.
En el archivo `Main.java` se realiza una transacción donde se crean varias entidades a modo
de demostración del funcionamiento del proyecto. 
## Ejecución del proyecto
Los pasos 2 y 3 pueden omitirse si tu IDE provee plug-ins que se encarguen de las dependencias del proyecto y permitan
ejecutarlo. 
1. **Clonar el repositorio.**
```sh
git clone https://github.com/jpbiondo/trabajo-practico-envers.git
cd trabajo-practico-envers
```
2. **Contruir el proyecto.** Para armar el proyecto, instalar las dependencias requeridas:
```sh
./gradlew build
```
3. **Correr el projecto.**
```sh
./gradlew run
```
## Dependencias
Este proyecto utiliza las siguientes dependencias:
- **[Hibernate](https://hibernate.org/)**: Implementación de JPA para persistir y mapear objetos a entidades del modelo relacional de base de datos.
- **[H2](https://www.h2database.com/html/main.html)**: Una base de datos ligera donde se persistirán las entidades.
- **[Lombok](https://projectlombok.org/)**: Librería que permite desintoxicar al proyecto de código como getters, setter y constructores.


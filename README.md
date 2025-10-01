# InnovaManager for ADSO

_InnovaManager for ADSO_ es un sistema de gestión integral desarrollado con **Spring Boot**, **MongoDB Atlas** y **MySQL**.  
El objetivo es administrar empleados, proyectos y asignaciones de manera centralizada, con exportación de datos (Excel/PDF) y un front-end responsivo con **Bootstrap + Thymeleaf**.

## 1. Requisitos previos

Antes de instalar y ejecutar el proyecto, asegúrate de tener lo siguiente instalado en tu máquina:

- **Java 17** o superior  
- **Apache Maven 3.9+**  
- **MySQL 8.x** con base de datos configurada  
- **MongoDB Atlas** o instancia local de MongoDB  
- **IDE recomendado**: IntelliJ IDEA o Eclipse con soporte para Spring Boot  

---

## 2. Instalación

1. Clonar este repositorio:  
   ```bash
   git clone https://github.com/tu-usuario/innova-manager.git
   cd innova-manager
   ```

2. Configurar las variables de entorno y credenciales en el archivo `application.properties` ubicado en `src/main/resources/`:  
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/innova_manager
   spring.datasource.username=tu_usuario
   spring.datasource.password=tu_password

   spring.data.mongodb.uri=mongodb+srv://usuario:password@cluster.mongodb.net/innova_manager
   ```

3. Instalar dependencias con Maven:  
   ```bash
   mvn clean install
   ```

---

## 3. Ejecución

Puedes ejecutar la aplicación de dos formas:  

- Usando Maven:  
  ```bash
  ./mvnw spring-boot:run
  ```

- O generando el JAR y ejecutándolo:  
  ```bash
  java -jar target/CRUDMIXTO-0.0.1-SNAPSHOT.jar
  ```

---

## 4. Pruebas

Una vez corriendo la aplicación, accede en tu navegador:  

- [http://localhost:8080](http://localhost:8080) → Página principal  
- [http://localhost:8080/empleados](http://localhost:8080/empleados) → Gestión de empleados  
- [http://localhost:8080/proyectos](http://localhost:8080/proyectos) → Gestión de proyectos  
- [http://localhost:8080/asignaciones](http://localhost:8080/asignaciones) → Gestión de asignaciones y tareas  

---

## 5. Créditos

Proyecto desarrollado por el equipo **DAMIAN Y EQUIPO DE TRABAJO* de la empresa **InnovaManager**:  

- Felipe Ramos  
- Alejandro Ortiz  
- Damian Martinez  

---

## 6. Licencia

Este proyecto es propiedad de **InnovaManager** y fue desarrollado con fines académicos y de gestión empresarial.  
Queda prohibida su distribución sin autorización del equipo de desarrollo.

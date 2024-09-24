# Proyecto de Microservicios con Spring Cloud
Este proyecto es un ejemplo de arquitectura de microservicios utilizando Spring Cloud con las siguientes tecnologías:

Spring Boot para la configuración de los microservicios.
Eureka Server como servicio de descubrimiento de microservicios.
Feign Client para facilitar la comunicación entre los microservicios.
Config Server para gestionar la configuración centralizada de los microservicios.
Requisitos Previos
Para ejecutar este proyecto, necesitas tener instalados los siguientes programas:

Java 17 o superior
Maven 3 o superior
Docker (Opcional, para desplegar los servicios de manera fácil)
Módulos del Proyecto
El proyecto está dividido en varios módulos/microservicios:

1. Eureka Server
Servicio de descubrimiento para registrar y localizar otros microservicios.

Directorio: /eureka-server
Puerto predeterminado: 8761

2. Config Server
Servidor centralizado para manejar la configuración de los microservicios.

Directorio: /configurations
Puerto predeterminado: 8888
Notas: La configuración se toma desde un repositorio Git, asegúrate de definir la URL correcta en el application.properties.


3. Microservicio 1 (Ejemplo: Servicio de Cursos)
Microservicio que maneja el catálogo de cursos con Eureka y Config Server.

Puerto predeterminado: 9090

4. Microservicio 2 (Ejemplo: Servicio de Estudiantes)
Microservicio encargado de gestionar estudiantes.
Puerto predeterminado: 8090

6. API Gateway
Gateway para gestionar el enrutamiento de peticiones hacia los diferentes microservicios.

Directorio: /api-gateway
Puerto predeterminado: 8080

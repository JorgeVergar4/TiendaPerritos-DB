# Tienda de Perritos - Base de Datos (AWS ECS Fargate)

Este repositorio contiene la configuracion y los scripts de persistencia para la capa de datos de la aplicacion Tienda de Perritos.

## Descripcion del Proyecto
Se utiliza una imagen personalizada de MariaDB/MySQL 8, la cual incluye la inicializacion automatica de la base de datos, tablas y registros base. El servicio esta orquestado en Amazon ECS bajo el modelo Fargate.

## Componentes del Repositorio
- Dockerfile: Configuracion de la imagen base y variables de entorno iniciales.
- init.sql: Script de estructuracion de datos (DDL y DML).

## Automatizacion y Despliegue
La gestion de la imagen se realiza mediante un pipeline de CI/CD en GitHub Actions, el cual automatiza el proceso de actualizacion en Amazon ECR y el redespliegue de la tarea en ECS.

### Redespliegue Manual
1. Acceder a la pestaña "Actions".
2. Seleccionar "CI/CD Tienda Perritos - DB (ECS)".
3. Ejecutar mediante "Run workflow".

---
Desarrollado por Jorge Vergara y Fernando Villalon - Evaluacion Parcial N°3 - Ingenieria DevOps.

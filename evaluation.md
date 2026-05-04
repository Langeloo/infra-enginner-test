# Prueba técnica Infrastructure Enginner I

## Duración estimada

Entre 2 y 3 horas.

## Formato de entrega

Prueba práctica desarrollada en un repositorio Git personal del candidato, entregado mediante enlace. Debe incluir:

* Código fuente.
* Instrucciones de ejecución en un README.
* Explicación breve de decisiones técnicas.
* Evidencia de pruebas ejecutadas.

## Estructura de la prueba

### Pasos previos

1. Crear una base de datos relacional (SQLite, PostgreSQL o MySQL) para la aplicación.
2. Crear una estrategia de insersion de los datos contenidos en el archivo [`data.json`](./data.json) a la base de datos relacional, utilizando un script o comando personalizado.

### Parte 1: Desarrollo backend

Construir una API sencilla en Django o Django REST Framework para gestionar una entidad, con productos, ordenes, entregas.

#### Requerimientos mínimos

* CRUD completo.
* Persistencia en una base de datos relacional (SQLite, PostgreSQL, MySQL).
* Al menos una consulta optimizada o filtro avanzado.
* Validaciones básicas de negocio.
* Endpoint adicional que consulte o consolide información desde una base de datos no relacional (MongoDB o Redis, según el escenario propuesto).

#### Ejemplo de escenario

Registrar órdenes de compra y almacenar en MongoDB un historial de eventos o auditoría asociado a cada orden, ademas el software debe soportar modo MULTITENANT.

### Parte 2: Contenedorización

* Crear un `Dockerfile` funcional para la aplicación.
* Definir un `docker-compose.yml` que levante la aplicación y sus dependencias.
* Incluir variables de entorno y buenas prácticas básicas de construcción.

### Parte 3: Automatización y CI/CD

* Configurar un pipeline en GitHub Actions.
* Ejecutar al menos:

  * Instalación de dependencias.
  * Linting.
  * Pruebas unitarias básicas.
  * Construcción de la imagen Docker.

### Parte 4: Infraestructura y operaciones (Bonus)

Responder brevemente preguntas prácticas o incluir archivos de ejemplo:

* Manifiesto básico de Kubernetes para desplegar la aplicación (`Deployment` y `Service`).
* Explicación de cómo escalar horizontalmente la aplicación.
* Comandos Linux para diagnóstico básico.

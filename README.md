# DOCKER

Curso de Docker - Guia practica de uso para los desarrolladores

## ¿Qué es Docker? y ¿Por qué debo de saberlo?

Docker es una plataforma de software que permite crear, probar y desplegar aplicaciones rápidamente mediante el uso de contenedores. Los contenedores son entornos ligeros y portátiles que incluyen todo lo necesario para ejecutar una aplicación, asegurando que funcione de manera consistente en cualquier sistema.

Aprender Docker es importante porque facilita la gestión de dependencias, mejora la portabilidad de las aplicaciones y optimiza el uso de recursos. Además, es ampliamente utilizado en la industria para el desarrollo, pruebas y despliegue continuo de software.

**Beneficios**:

- Cada contenedor está aislado de los demás.
- Es posible ejecutar varias instancias de la misma versión o diferentes versiones sin configuraciones adicionales.
- Con un comando, puedes descargar, levantar y correr todo lo que necesitas.
- Cada contenedor contiene todo lo que necesita para ejecutarse.
- Indifirente del sistema operativo HOST.

## Comandos

**Image - Imagen de contenedor**: Es un archivo construido por capas, que contiene todas las dependencias para ejecutarse, tal como: las dependencias, con guraciones, scripts, archivos binarios, etc.

**Docker Deamon**: Es el servicio en segundo plano que se ejecuta en el host que administra la creación, ejecución y distribución de contenedores Docker.

**Container**: Es una instancia de una imagen ejecutándose en un ambiente aislado.

### Comandos básicos de Docker

| Comando                | Descripción                                                                                                |
| ---------------------- | ---------------------------------------------------------------------------------------------------------- |
| `docker pull`          | Descarga una imagen desde Docker Hub. Ejemplo: `docker pull nginx`                                         |
| `docker container run` | Crea y ejecuta un contenedor a partir de una imagen. Ejemplo: `docker container run name-image`            |
| `docker ps`            | Lista los contenedores en ejecución. Usa `docker ps -a` para ver todos, incluidos los detenidos.           |
| `docker images`        | Muestra las imágenes descargadas en tu sistema.                                                            |
| `docker build`         | Construye una imagen a partir de un Dockerfile.                                                            |
| `docker stop`          | Detiene un contenedor en ejecución. Ejemplo: `docker stop nombre_contenedor`                               |
| `docker rm`            | Elimina un contenedor detenido.                                                                            |
| `docker rmi`           | Elimina una imagen.                                                                                        |
| `docker exec`          | Ejecuta un comando dentro de un contenedor en ejecución. Ejemplo: `docker exec -it nombre_contenedor bash` |
| `docker logs`          | Muestra los registros (logs) de un contenedor.                                                             |
| `docker ls ( -a)`      | Muestra todos los contenedores que por defecto estan ejecutandose, con el (-a) los muestra todos           |

> Estos son los comandos más usados. Docker tiene muchos más, pero con estos puedes empezar a trabajar y gestionar contenedores de manera eficiente.

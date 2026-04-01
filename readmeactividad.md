Propósito del repositorio
Este repositorio contiene los archivos necesarios para el laboratorio de DevOps. El objetivo principal es tener el código versionado para automatizar la creación de una imagen Docker usando GitHub Actions (CI/CD). Esta imagen, que levanta un servidor web básico con Nginx, será la que usaremos después para probar la infraestructura de red de 3 capas (web, app, datos) que se va a configurar en AWS.

Estrategia de control de versiones
Para hacer este proyecto estoy usando una estrategia de Ramas de Características (Feature Branches). Esto significa que no se programa directamente en la rama principal. En lugar de eso, dividí el trabajo inicial en tres ramas independientes:

feature/frontend: donde está el archivo index.html con el "Hola Mundo".

feature/docker: donde está el Dockerfile basado en la imagen de nginx:alpine.

feature/docs: donde escribí este README.md.

Una vez listas, cada una de estas ramas se integra a la rama main a través de Pull Requests separados.
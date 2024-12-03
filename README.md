# TrabajoFinal
# Proyecto de Integración Continua
Este repositorio contiene la configuración de un proyecto que integra:
- Contenedores con Docker.
- Jenkins, Travis CI y Codeship para CI/CD.
- Monitoreo de errores con Sentry.
# Ramas
Si se utilizan diferentes Ramas

main:

Propósito: Es la rama principal y contiene el código estable y listo para producción. Esta rama solo debe tener código que haya sido completamente probado y validado.
Uso: Es la rama de referencia que refleja el estado final del proyecto, y es la que se despliega en producción. Solo se realiza un merge hacia main desde otras ramas cuando el código está listo para producción.
Estrategia: Debe ser protegida para evitar cambios directos. Los cambios en main siempre deben venir de un merge desde develop o desde una rama feature.

develop:

Propósito: Es la rama donde se integran los cambios en desarrollo. Es el punto de partida para cualquier nueva funcionalidad o corrección, y se considera la rama de trabajo principal para el desarrollo.
Uso: Aquí es donde se fusionan las ramas feature después de ser probadas y revisadas. No se debe desplegar directamente desde develop; en su lugar, se realiza un merge a main cuando se tiene una versión estable.
Estrategia: Sirve como la base para todas las ramas de características (feature), y cualquier nueva funcionalidad o corrección se integra primero aquí.

# Participacion
Este trabajo lo hago solo.
## Estructura del Proyecto
- `docker/docker-compose.yml`: Configuración de contenedores.
- `Jenkinsfile`: Pipeline de Jenkins.
- `.travis.yml`: Configuración de Travis CI.
- `README.md`: Detalles del proyecto.

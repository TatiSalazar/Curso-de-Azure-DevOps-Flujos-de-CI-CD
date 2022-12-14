# Curso de Azure DevOps Flujos de CI CD

## ¿Qué es DevOps?
* Es una cultura
* Se relaciona 2 componentes: Desarrollo y Operaciones
* Aparece en 2009 el concepto
* Cultura de mejora continua que involucra cada uno de los aspectos de TI y procesos de desarrollo
* Se enfoca en procesos, personas y herramientas
* No confundir con: Un puesto de trabajo, una herramienta, metodologia agil, tecnologia, un rol.

## DevOps va de la mano con 
* El Agilismo
* Automatizacion
* Soporte de Infraestructura
* Integracion continua y despliegue continuo

## Ciclo de vida DevOps
* plan -> code -> build -> test -> release -> deploy -> operate -> monitor ->
* plan : azure boards
* code: azure repos
* build, test : azure pipeline
* deploy, operate: azure artifacts
* monitor : azure test plans

## Azure Boards
* Herramienta de planeacion agil
* Seguimiento del trabajo con paneles kanban, registros de trabajo
* Registros de tareas, sprint, etc.

# Azure Repos
* Repositorios privados gratuitos ilimitados
* Manejar los repositorios con los files, commits, Pull Request
* Consiga un excelente hospedaje GIT, flexible y con revisiones de codigo muy eficaces

## Azure Pipelines
* CI/CD para cualquier plataforma
* Ayuda con la integracion
* Compila, pruebe e implemente soluciones con cualquier lenguaje, en cualquier nube o en local.
* Ejecuta archivos en paralelo con linux, macOs, Windows
* Implementar contenedores en hosts indivuduales o en Kubernets

## Azure Test Plans 
* QA Calidad
* Prueba manuales y exploratorias
* Realizar pruebas periodicas y publicar versiones con confianza
* Mejora la calidad del codigo con herramientas de prueba manueales y exploratorias para sus aplicaciones.
* Es de pago, es costoso

## Azure Artifacts
* Repositorio de paquetes universal
* Comparta paquetes maven, npm, NuGet y Python de origineses publicos y privados con todo su equipo.

## Estructura Organizacional
* Nuestra Cuenta de Azure DevOps puede tener multiples organizaciones.
* Una Organizacion es un grupo de proyectos que estan relacionados entre si.
* Podemos hacer parte de Organizaciones externas mediante una invitacion, para trabajar en proyectos externos.

## Azure DevOps Server
* (Azure DevOps en tu propia infraestructura). Esta versión nos permite Instalar en nuestra propia Infraestructura los servicios de Azure DevOps con un esfuerzo bastante grande y limitada, debe ser considerada por seguridad o políticas de compañía. El licenciamiento se da por usuario o por servicios Individuales.

## Recursos para aprender DevOps:
* https://dev.to/t/devops
* https://devopsdays.org/
* https://azuredevopslabs.com/
* https://docs.microsoft.com/learn/paths/evolve-your-devops-practices/

## Pagina oficial 
https://dev.azure.com/

# Permisos, accesos, ay seguridad 
https://docs.microsoft.com/en-us/azure/devops/organizations/security/about-permissions

## Creando Ramas y Pull Request
* Básicamente un pull request es una petición para integrar nuestras propuestas o cambios de código a un proyecto.
* Una buena práctica de ramas es no hacer PR directos a master, los desarrolladores debemos trabajar con una estructura logica que puede variar pero lo más (basico) común es:
- Master
- Release
- Develop
- Features
- Hotfix
* Features y Hotfix son las ramas de un desarrollador, los PR se hacen desde estas ramas hacia develop, los cuales deben ser revisados por un code reviewer.

## Pipeline
* Básicamente un pipeline es una secuencia de comandos que hacen una ejecución de la aplicación, para poder comprobar que esta funcionando, compilando, que corran las pruebas unitarias, es decir que esta lista para poderse mover a la siguiente fase o ciclo de desarrollo que es la publicación.

## Configurar el pipeline:
* Se selecciona el framework
* trigger: se dispara desde master
* pool: el agente que se usa, ejemplo, ubuntu
* steps, task: la primera tarea que se va a ejecutar

* Pasos:
* 1. Pipelines
* 2. Azure Repos Git YAML
* 3. Configure your pipeline : Node with React
* 4. Review your pipeline YAML

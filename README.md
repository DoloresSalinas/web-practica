# Implementación de Landing Page con CI/CD en GitHub Pages

Este proyecto consiste en implementar una landing page estática y automatisar tanto su construcción como su despliegue utilizando ** CI/DI con GitHub Actions**. Esto significa que, cada vez que se realice un cambio en el repositorio, el flujo de trabajo se encarga de compilar el proyecto y publicar automáticamente la última versión en Github Pages, sin intervención manual, facilitando así el mantenimiento y la actualización del sitio.

## Características

- Implementa una landing page estática.
- La aplicación se despliega automáticamente en Github Pages cada vez que se hace un nuevo push a la rama principal.
- Utiliza un flujo de integración y despliegue continuos (CI/DI) con Github Actions, sin intervención manual.
- La aplicación está construida con React.- Utiliza Node.js para instalar dependencias y ejecutar el entorno de desarrollo.
- La aplicación se distribuye sin necesitar un backend.
## Tecnologías utilizadas

- Github (para el control de versiones)
- Github Actions (para CI/DI)
- Github Pages (para el despliegue)
- HTML, CSS y JavaScript (para el diseño y funcionamiento de la landing page)
- React como framework
- Node versión 22.14.0
- YAML (para la configuración del flujo de trabajo de CI)

## Estructura general del Proyecto
web-practica/
 └ .github/
 |  └ workflows/
 |    └ ci-cd.yaml
 └ src/
 |  └ App.jsx
 └ public/
 └ .gitignore
 └ .nojekyll
 └ package-look.json
 └ package.json 
 └ README.md

Descripción de cada elemento:
✅ .github/
Contiene la configuración de GitHub Actions.
Dentro de workflows encuentras el flujo de CI-CD que se encarga de crear y desplegar automáticamente tu aplicación en GitHub Pages.

✅ ci-cd.yaml
Archivo de configuración de GitHub Actions donde se definen los trabajos de construcción, pruebas y despliegue de tu aplicación React.

✅ src/
Carpeta principal del código fuente de tu aplicación React.

✅ App.jsx
Componente principal de tu aplicación React.
Generalmente aquí empieza el árbol de componentes de la aplicación.

✅ public/
Archivos estáticos que se incluyen directamente en el build (imágenes, iconos, manifest, index.html...).
Esta carpeta suele funcionar como “raíz” de tu aplicación en el navegador.

✅ .gitignore
Archivo que especifica qué archivos o carpetas se ignoran en el control de versiones (por ejemplo, node_modules) para evitar que sean enviados al repositorio.

✅ package-lock.json
Generado automáticamente por npm.
Almacena las versiones exactas de cada dependencia para que el proyecto pueda instalarse de forma reproducible en diferentes entornos.

✅ package.json
Describe tu aplicación, sus dependencias, sus scripts de inicio, construcción, pruebas, etc.

✅ .nojekyll
Este pequeño fichero sin contenido evita que GitHub Pages invoque Jekyll, que podría interferir con el despliegue de tu aplicación React.

✅ README.md
Proporciona una guía para que cualquier nuevo desarrollador pueda instalar, ejecutar o dar mantenimiento a tu aplicación.

## Instalación

1. Clona el repositorio:
- git clone https://github.com/DoloresSalinas/web-practica.git
- cd web-practica

2. Asegúrate de tener Node instalado, puedes ver la versión con el comando:
- node --version

3. Instala las dependencias del proyecto:
- npm install

4. Inicia el servidor de desarrollo:
- npm start

5. Accede a la aplicación en tu navegador:
- http://localhost:3000

Despliegue en GitHub Pages
Cada nuevo push a la rama principal despliega automáticamente la aplicación en GitHub Pages.
Puedes acceder a ella en:
- https://DoloresSalinas.github.io/web-practica/

## Autor
- María Dolores Salinas Jiménez




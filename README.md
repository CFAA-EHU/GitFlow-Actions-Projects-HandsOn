# GitFlow-Actions-Projects-HandsOn

Repositorio para aprender y practicar un flujo de trabajo basado en **GitFlow** usando GitHub.

## Objetivo

Este repositorio está pensado como apoyo para talleres o prácticas en las que se quiere aprender a:

- trabajar con ramas `main` y `develop`
- crear ramas de funcionalidad (`feature/*`)
- preparar versiones (`release/*`)
- corregir incidencias urgentes (`hotfix/*`)
- apoyar el trabajo con GitHub Projects y GitHub Actions

## Flujo recomendado

### Ramas principales

- `main`: contiene el código estable o publicado
- `develop`: integra el trabajo en curso antes de llegar a `main`

### Ramas auxiliares

- `feature/<nombre>`: para desarrollar una nueva funcionalidad a partir de `develop`
- `release/<version>`: para preparar una entrega desde `develop`
- `hotfix/<nombre>`: para corregir un problema urgente a partir de `main`

## Ejemplo de trabajo con GitFlow

1. Crear una rama de trabajo desde `develop`:

   ```bash
   git checkout develop
   git checkout -b feature/mi-cambio
   ```

2. Realizar los cambios y confirmarlos:

   ```bash
   git add .
   git commit -m "Añade una mejora"
   ```

3. Integrar la rama en `develop` mediante una pull request.

4. Cuando el conjunto de cambios esté listo para una entrega, crear una rama `release/*`.

5. Tras validar la release, fusionarla en `main` y de vuelta en `develop`.

## Qué practicar en este repositorio

- apertura y cierre de ramas siguiendo GitFlow
- resolución de conflictos sencillos
- uso de pull requests
- seguimiento del trabajo con GitHub Projects
- automatización básica con GitHub Actions

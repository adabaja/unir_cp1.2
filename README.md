# Caso Práctico 1.2 - DevOps & Cloud

Repositorio del CP1.2 del curso Experto Universitario en DevOps & Cloud (UNIR).

El proyecto es una calculadora en Python con API REST usando Flask. Lo uso para montar un pipeline de CI en Jenkins con distintos tipos de pruebas.

## Qué incluye

- `app/` - la calculadora y la API
- `test/unit/` - pruebas unitarias
- `test/rest/` - pruebas de integración
- `test/jmeter/` - pruebas de rendimiento
- `test/wiremock/` - mock para las pruebas REST
- `Jenkinsfile` - pipeline principal
- `JENKINSFILE_agentes` - pipeline distribuido en 3 agentes

## Ramas

- `master` - rama principal
- `feature_fix_coverage` - mejora de cobertura al 100%

## Notas

- Se uso un nuevo _ENV_ `conda activate unir_devops`.
- Se instalo los paquetes necesarios `pip install pytest flask flake8 bandit coverage`
- Se instalo Jenkins y jmeter usando el *brew* porque estoy usando MAC. `brew install jenkins-lts` & `brew install jmeter`
- Gihub conectado por SSH a mi macbook, no es necesario usar tokens.

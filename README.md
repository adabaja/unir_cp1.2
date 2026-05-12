# Caso Práctico 1.2 - DevOps & Cloud

Repositorio del CP1.2 del curso Experto Universitario en DevOps & Cloud (UNIR).

El proyecto es una calculadora en Python con API REST usando Flask. Lo uso para montar un pipeline de CI en Jenkins con distintos tipos de pruebas.

## Qué incluye

- `app/` - la calculadora y la API
- `test/unit/` - pruebas unitarias
- `test/rest/` - pruebas de integración
- `test/jmeter/` - pruebas de rendimiento
- `test/wiremock/` - mock para las pruebas REST
- `JENKINSFILE` - pipeline principal
- `JENKINSFILE_agentes` - pipeline distribuido en 3 agentes

## Notas

- Se uso un nuevo _ENV_ `conda activate unir_devops`.
- Se instalo los paquetes necesarios `pip install pytest flask flake8 bandit coverage pip-audit`
- Se instalo Jenkins y jmeter usando el *brew* porque estoy usando MAC. `brew install jenkins-lts` & `brew install jmeter`
- Github conectado por SSH a mi macbook, no es necesario usar tokens.

## To Do

- Deberia usar el paquete de pip-audit como fase en jenkins --> Auditar los paquetes
- hacer el *JENKINSFILE* deberia agregar qualityGate para pip check y pip-audit? o mejor mando lo que pide el reto 1 -> si termino antes los retos 2 y 3 lo agrego como experimento. 
- hacer el *JENKINSFILE_agentes*

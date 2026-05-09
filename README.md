# CP1.2 – Pipeline CI con Jenkins

Proyecto de la asignatura **Experto Universitario en DevOps & Cloud**.

## Descripción

Aplicación Python de calculadora con microservicios Flask, utilizada como base para practicar
integración continua con Jenkins. Incluye pruebas unitarias, de integración, análisis estático,
seguridad, cobertura y rendimiento.

## Estructura

```
app/          → Librería calculadora + API Flask
test/unit/    → Pruebas unitarias (pytest)
test/rest/    → Pruebas de integración REST
test/jmeter/  → Plan de pruebas de rendimiento (JMeter)
test/wiremock/→ Mock para endpoint sqrt
```

## Herramientas

- Python 3 + pytest, flask, flake8, bandit, coverage
- Jenkins (JUnit, Warnings-NG, Coverage, Performance)
- JMeter
- Wiremock

## Ramas

- `master` → código estable (Reto 1 y 2)
- `feature_fix_coverage` → cobertura 100% (Reto 3)

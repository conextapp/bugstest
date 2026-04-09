# BugTest - Pruebas Maestro para Conext App

## Requisitos
- Maestro CLI instalado (`npm i -g maestro`)
- Dispositivo móvil real conectado (ID: njwo455x6lx895kb)
- App `com.conextapp.mobile` instalada

## Ejecutar Tests

```bash
# Desde PROYECTO/maestro-test
maestro test --local
```

## Estructura
- `common/` - Flujos reutilizables (login, etc.)
- `tests/` - Tests individuales que usan los flujos de common

## Notas
- El swipe de 10s es para grabación de video local
- Coordenadas verificadas en móvil real
# Equipo 27 - SoftCrédito

Repositorio del proyecto **"SoftCrédito – Probabilidad de Incumplimiento"**.

## Contenido
- `Avance2Equipo27.ipynb`: cuaderno con el primer avance de análisis y limpieza de datos.
- `docker-compose.yml`: define el contenedor MySQL utilizado para cargar la base.
- `.gitignore`: excluye archivos `.sql` generados localmente.

## Requisitos
- Docker y Docker Compose.
- Jupyter Notebook o JupyterLab para ejecutar el cuaderno.

## Uso rápido
1. Levantar la base de datos local:
   ```bash
   docker-compose up -d
   ```
   Esto crea el contenedor `mysql_softcred` (puerto `3306`). Credenciales por defecto:
   - usuario: `analyst`
   - contraseña: `analystpass`
   - base: `BASE1`

   El directorio `softcred_BASE1_clean` debe contener los scripts SQL de inicialización (no incluido en este repositorio).

2. Abrir el cuaderno Jupyter:
   ```bash
   jupyter notebook Avance2Equipo27.ipynb
   ```
   Siga las celdas para replicar el proceso de conexión, limpieza y análisis exploratorio.

3. Cuando termine, detener los servicios:
   ```bash
   docker-compose down
   ```

## Objetivo del proyecto
Desarrollar un modelo robusto para predecir el incumplimiento crediticio empleando aprendizaje automático. El cuaderno actual documenta la preparación de datos y los primeros hallazgos.

## Contribuciones
Se agradecen sugerencias y _pull requests_. Para reportar problemas o solicitar mejoras, abra un issue.

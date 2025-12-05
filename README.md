# VisionArtificial
Este repositorio será utilizado para afianzar los conocimientos de Visión Artificial y hacer proyectos.

## Inicialicación
- Activar el entorno virtual
  ```sh
  source venv/bin/activate
  ```

- Abrir el jupyter notebook
  ```sh
  jupyter notebook
  ```

## Estructura de carpetas
- `notebooks/`: cuadernos por bloque/tema (ej: `bloque01_fundamentos.ipynb`) con varias secciones dentro.
- `src/`: utilidades reutilizables (IO, visualización, transformaciones, métricas) para no duplicar código entre notebooks.
- `data/`: datos centralizados.
  - `raw/`: originales sin modificar.
  - `processed/`: derivados (recortes, redimensionados, normalizados).
  - `labels/`: anotaciones y splits.
- `models/`: pesos/checkpoints descargados o entrenados, configs asociadas.
- `outputs/`: resultados de experimentos (imágenes/vídeos con overlays, métricas, gráficos) organizados por fecha o bloque.

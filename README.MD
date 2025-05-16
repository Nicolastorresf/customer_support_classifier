# Proyecto de Clasificación de Mensajes de Soporte al Cliente para Nequi

Este proyecto es una solución para la prueba técnica de Ingeniero de Machine Learning de Nequi. El objetivo es diseñar y construir un pipeline de ML para clasificar mensajes de usuarios enviados a un canal de atención al cliente.

## Descripción General

El sistema ingiere mensajes de texto, los procesa, y utiliza un modelo de Machine Learning para clasificarlos en categorías predefinidas (ej: "Consulta General", "Problema Técnico", "Feedback Producto"). La solución está diseñada siguiendo las mejores prácticas de MLOps, incluyendo versionamiento, pruebas, orquestación y propuestas de monitoreo y seguridad en un entorno batch.

## Estructura del Repositorio (Propuesta Inicial)
nequi_ml_challenge/
├── data/                     # Almacenamiento de datos (crudos, procesados, etc. - usar .gitignore para datos grandes)
│   ├── raw/                  # Datos crudos originales
│   └── processed/            # Datos después del preprocesamiento
├── notebooks/                # Jupyter notebooks para exploración (EDA) y experimentación
├── src/                      # Código fuente del proyecto
│   ├── init.py
│   ├── data_ingestion.py     # Scripts para la ingesta de datos
│   ├── data_processing.py    # Scripts para la limpieza y transformación de datos
│   ├── model_training.py     # Script para el entrenamiento del modelo
│   ├── model_inference.py    # Script para la inferencia batch
│   ├── utils.py              # Funciones de utilidad
│   └── config.py             # Configuraciones del proyecto (paths, parámetros)
├── tests/                    # Pruebas unitarias e de integración
├── models/                   # Modelos entrenados y serializados (ej: .pkl, .joblib)
├── reports/                  # Reportes generados (ej: métricas de evaluación, visualizaciones EDA)
├── .github/                  # Workflows de GitHub Actions para CI/CD
│   └── workflows/
│       └── main.yml
├── .gitignore                # Especifica archivos y directorios a ignorar por Git
├── requirements.txt          # Dependencias del proyecto Python
└── README.md                 # Este archivo

## Roadmap y Fases (Resumen)

1.  **Fase 1: Inmersión, Selección de Datos y Diseño Inicial (Día 1)**
    * [x] Comprensión del problema
    * [x] Selección del Dataset: Customer Support on Twitter
    * [ ] Definición preliminar de categorías
    * [x] Esbozo arquitectónico inicial (ver sección abajo)
    * [x] Repositorio de GitHub creado con README.md inicial
2.  **Fase 2: Pipeline de Procesamiento de Datos e Implementación del Modelo Base (Días 2-3)**
3.  **Fase 3: Diseño Detallado de Arquitectura en la Nube y Orquestación (Día 4)**
4.  **Fase 4: Implementación de CI/CD/CT, Propuesta de Monitoreo y Seguridad (Días 5-6)**
5.  **Fase 5: Pruebas, Documentación Final, Refinamiento y Entrega (Día 7)**

## Esbozo Arquitectónico Inicial (Alto Nivel)

*Se describirá en la siguiente sección de este README o en un archivo `docs/architecture.md`.*

## Configuración y Ejecución

*(Se completará a medida que se desarrolle el proyecto)*

1.  Clonar el repositorio: `git clone <URL_DEL_REPOSITORIO>`
2.  Crear y activar un entorno virtual:
    ```bash
    python -m venv venv
    source venv/bin/activate  # En Windows: venv\Scripts\activate
    ```
3.  Instalar dependencias: `pip install -r requirements.txt`
4.  Ejecutar el pipeline: `python src/main.py` (o similar, por definir)

## Decisiones de Diseño y Justificaciones

*(Se documentarán aquí las decisiones clave tomadas durante el proyecto)*
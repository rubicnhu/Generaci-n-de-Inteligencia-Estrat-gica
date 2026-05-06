# Predicción de la Delincuencia en Barcelona: Enfoque Multidelictivo para 2026

Este repositorio contiene el código fuente, los modelos y el análisis desarrollado para el proyecto de investigación sobre la criminalidad urbana en Barcelona, utilizando técnicas de Machine Learning para proyectar escenarios en 2026.

## 📌 Descripción del Proyecto

El objetivo de este trabajo es desarrollar un sistema predictivo capaz de anticipar tendencias delictivas por distritos. Para ello, se integra información histórica de hechos penales con variables sociodemográficas y dinámicas urbanas, validando visualmente el uso de datos bajo teorías criminológicas como la **Teoría de las Actividades Rutinarias** y la **Teoría del Patrón Delictivo**.

## 🚀 Metodología y Modelado

El pipeline de datos incluye la extracción desde **Open Data BCN**, ingeniería de características avanzada (lags temporales, medias móviles) y un torneo de algoritmos para identificar la arquitectura más robusta.

### Comparativa de Rendimiento

Se evaluaron múltiples modelos bajo la métrica **MAPE (Mean Absolute Percentage Error)**:

| Algoritmo | MAPE | Estado |
| :--- | :--- | :--- |
| **LightGBM** | **5,86 %** | **Modelo Definitivo** (Optimizado con Leaf-wise growth) |
| SVM (Support Vector Machines) | 7,17 % | Rendimiento competitivo tras Grid Search |
| XGBoost / Random Forest | 7,00 - 10,00 % | Algoritmos base |
| TFT (Temporal Fusion Transformer) | ~20,00 % | Ineficaz por volumen de datos limitado |

## 📂 Estructura del Repositorio

* `data/`: Datasets procesados y normalizados.
* `scripts/`: Código fuente de los algoritmos.

## 🛠️ Instalación y Uso

1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/tfm-barcelona-crime.git](https://github.com/tu-usuario/tfm-barcelona-crime.git)

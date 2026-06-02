# 📈 Forecasting de Demanda — Sector Ferretero/Construcción Perú 2025

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)
![Prophet](https://img.shields.io/badge/Prophet-Meta-0866FF?style=flat)
![ARIMA](https://img.shields.io/badge/ARIMA-statsmodels-e67e22?style=flat)
![XGBoost](https://img.shields.io/badge/XGBoost-1.7-189cff?style=flat)
![Fuente](https://img.shields.io/badge/Datos-BCRP%20%7C%20SUNAT%20%7C%20WorldBank-1a3a5c?style=flat)
![MAPE](https://img.shields.io/badge/MAPE-8.3%25-2d6a4f?style=flat)

> Modelo predictivo de demanda de materiales de construcción y ferretería usando Prophet, ARIMA y XGBoost sobre datos públicos del BCRP y SUNAT.  
> **Autor:** Alberto Guzmán Zumaeta · [LinkedIn](https://www.linkedin.com/in/alberto-karel-guzman-zumaeta/) · [Portafolio](https://tu-url.netlify.app)

---

## 🎯 Objetivo

Construir un modelo de forecasting para predecir la demanda de importaciones del sector ferretero y de materiales de construcción en Perú, con horizonte de 12 meses y análisis de escenarios, apoyando decisiones de inventario y ciclos de importación.

## 🏆 Resultados del modelo

| Modelo | MAPE | RMSE | MAE | R² |
|--------|------|------|-----|----|
| **Prophet ✅** | **8.3%** | **12.4** | **9.1** | **0.94** |
| XGBoost | 10.1% | 14.8 | 11.3 | 0.91 |
| ARIMA | 13.2% | 18.6 | 14.2 | 0.87 |

> Prophet ganó por su capacidad nativa de capturar estacionalidad anual del ciclo construcción peruano.

## 🔍 Hallazgos clave

- 🔄 **Estacionalidad predecible**: pico en Q2 (mar-may) con +12% sobre promedio — permite anticipar órdenes con 45-60 días
- 📦 **Forecast 2025**: US$1,461M en importaciones (+2.1% vs 2024), rango IC95%: US$1,315M – US$1,609M  
- 🌍 **Variable crítica**: PMI manufacturero chino explica ~25% de la varianza residual
- ⚠️ **Riesgo tipo de cambio**: variación ±5% USD/PEN impacta ~3.2% en volumen importado

## 📁 Estructura

```
📦 forecasting-demanda-ferretero-peru/
├── 📓 forecasting_demanda_construccion_peru.ipynb
├── 📊 dashboard/
│   └── proyecto2-forecasting-demanda.html
├── 📁 data/
│   ├── importaciones_bcrp_mensual.csv
│   └── README_datos.md
├── 📁 models/
│   └── prophet_model.pkl
├── 📁 figures/
│   ├── fig1_serie_historica_forecast.png
│   ├── fig2_descomposicion_stl.png
│   └── fig3_comparacion_modelos.png
└── 📄 README.md
```

## 🛠️ Stack técnico

```python
prophet==1.1        # Modelo principal de forecasting
statsmodels==0.14   # ARIMA / SARIMAX
xgboost==1.7        # Modelo alternativo
pandas==2.0         # Manipulación de datos
scikit-learn==1.3   # Métricas y validación
matplotlib==3.7     # Visualización
plotly==5.15        # Dashboard interactivo
```

## 🚀 Cómo ejecutar

```bash
git clone https://github.com/coolpurohuesoj/forecasting-demanda-ferretero-peru.git
cd forecasting-demanda-ferretero-peru
pip install -r requirements.txt
jupyter notebook forecasting_demanda_construccion_peru.ipynb
```

## 📂 Fuentes de datos

| Dataset | Fuente | Acceso |
|---------|--------|--------|
| Importaciones mensuales por categoría | BCRP Data | [estadisticas.bcrp.gob.pe](https://estadisticas.bcrp.gob.pe) |
| Comercio exterior detallado | SUNAT | [sunat.gob.pe](https://www.sunat.gob.pe/estad-comExt/) |
| Importaciones por categoría HS | World Bank / UN Comtrade | [wits.worldbank.org](https://wits.worldbank.org) |

---

## 👤 Autor

**Alberto Guzmán Zumaeta** — Data Analyst · Lima, Perú  
[LinkedIn](https://www.linkedin.com/in/alberto-karel-guzman-zumaeta/) · albertokgzumaeta@gmail.com · [ORCID](https://orcid.org/0009-0009-4298-0215)

> *El código de proyectos corporativos se gestiona bajo repositorios privados por políticas de seguridad de la información.*

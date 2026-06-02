# 📊 Análisis del Mercado Laboral Peruano 2022–2024

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?style=flat&logo=pandas)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter)
![Fuente](https://img.shields.io/badge/Fuente-INEI%20EPEN-1a4731?style=flat)
![Licencia](https://img.shields.io/badge/Datos-Open%20Data%20ODbL-52b788?style=flat)

> Análisis exploratorio de indicadores del mercado laboral peruano 2022-2024 usando datos públicos del INEI.
> **Autor:** Alberto Guzmán Zumaeta · [LinkedIn](https://www.linkedin.com/in/alberto-karel-guzman-zumaeta/) · [Portafolio](https://tu-url.netlify.app)

---

## 🎯 Objetivo

Identificar tendencias y patrones en el mercado laboral peruano post-pandemia, analizando empleo, ingresos, informalidad y brechas de género a través de datos públicos del INEI.

## 📌 Preguntas de análisis

| # | Pregunta | Técnica utilizada |
|---|----------|-------------------|
| 1 | ¿Cómo se recuperó el empleo post-pandemia? | Series temporales, comparación YoY |
| 2 | ¿Qué relación hay entre educación e ingresos? | Correlación de Pearson, regresión |
| 3 | ¿Cómo evoluciona la informalidad por sector? | Análisis multivariado, benchmarking |
| 4 | ¿Cuál es el estado de la brecha de género? | Comparación de medias, proyección temporal |

## 🔍 Hallazgos principales

- 📈 **+2.8M empleos** recuperados desde el pico pandémico (2021→2024)
- ⚠️ **71.2% informalidad** con reducción de apenas 0.9pp en 2 años — problema estructural
- 💡 **Retorno educativo de 3.7x**: universitario (S/2,980) vs primaria (S/798)
- ⚖️ Brecha de género de **S/477/mes** — al ritmo actual, paridad en ~15 años

## 📁 Estructura del repositorio

```
📦 analisis-mercado-laboral-peru/
├── 📓 analisis_mercado_laboral_peru_2024.ipynb   # Notebook principal
├── 📊 dashboard/
│   └── mercado_laboral_peru.html                 # Dashboard interactivo
├── 📁 data/
│   └── README_datos.md                           # Instrucciones descarga INEI
├── 📁 figures/
│   ├── fig1_evolucion_mercado_laboral.png
│   ├── fig2_brecha_genero.png
│   └── fig3_informalidad_sectores.png
└── 📄 README.md
```

## 🛠️ Stack técnico

```python
pandas==2.0        # Manipulación de datos
numpy==1.24        # Operaciones numéricas
matplotlib==3.7    # Visualización estática
seaborn==0.12      # Visualización estadística
scipy==1.11        # Estadísticas y correlaciones
plotly==5.15       # Dashboard interactivo
```

## 🚀 Cómo ejecutar

```bash
# 1. Clonar repositorio
git clone https://github.com/coolpurohuesoj/analisis-mercado-laboral-peru.git
cd analisis-mercado-laboral-peru

# 2. Instalar dependencias
pip install -r requirements.txt

# 3. Descargar datos del INEI
# Ver instrucciones en data/README_datos.md

# 4. Abrir notebook
jupyter notebook analisis_mercado_laboral_peru_2024.ipynb
```

## 📂 Fuente de datos

| Dataset | Fuente | Período | Acceso |
|---------|--------|---------|--------|
| EPEN — Indicadores mercado laboral | INEI | 2020-2024 | [datosabiertos.gob.pe](https://datosabiertos.gob.pe) |
| Microdatos ENAHO | INEI | 2022-2024 | [proyectos.inei.gob.pe/microdatos](https://proyectos.inei.gob.pe/microdatos/) |
| Informe MTPE | MTPE-DISEL | Q1 2024 | [gob.pe](https://cdn.www.gob.pe/uploads/document/file/6653196/5783668-ite-2024-t1.pdf) |

**Licencia de datos:** Open Data Commons Open Database License (ODbL)
**Licencia del código:** MIT

---

## 👤 Autor

**Alberto Guzmán Zumaeta** — Data Analyst · Lima, Perú

- 🔗 [LinkedIn](https://www.linkedin.com/in/alberto-karel-guzman-zumaeta/)
- 📧 albertokgzumaeta@gmail.com
- 🔬 [ORCID](https://orcid.org/0009-0009-4298-0215)
- 📄 [Publicación académica — Revista Interfases ULIMA](https://doi.org/10.26439/interfases2023.n018.6625)

> *Este es uno de varios proyectos de análisis de datos públicos peruanos. El código de proyectos corporativos se gestiona bajo repositorios privados de cada empresa por políticas de seguridad de la información.*

# 📊 Análisis Global de Tuberculosis (Datos WHO & INEGI)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](TU_LINK_DE_COLAB_AQUI)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Library-Pandas-orange)

## 📖 Descripción del Proyecto
Este repositorio contiene un análisis detallado sobre la incidencia de la tuberculosis a nivel global, con un enfoque especial en la integración de datos de salud y demografía. El proyecto procesa grandes conjuntos de datos de la Organización Mundial de la Salud (WHO) y datos poblacionales para entender la evolución de la enfermedad en diferentes contextos.

El notebook está diseñado para ejecutarse íntegramente en **Google Colab**, aprovechando la integración con Google Drive para el manejo de archivos masivos.

---

## 🛠️ Tecnologías y Librerías
El análisis se apoya en el ecosistema científico de Python:
* **Pandas:** Para la manipulación, limpieza y "unpivoting" de las tablas de datos.
* **Numpy:** Para operaciones vectorizadas y manejo de valores nulos.
* **Google Colab/Drive:** Para el almacenamiento persistente de los datasets intermedios y finales.

---

## 📂 Estructura del Análisis
El código sigue un flujo lógico de ciencia de datos:
1.  **Carga de Datos:** Importación de datasets desde Google Drive (`population.csv` y `who.csv`).
2.  **Exploración Inicial:** Visualización de estructuras de datos y tipos de variables (iso2, iso3, años, casos por rango de edad y género).
3.  **Limpieza y Transformación:** (En proceso) Preparación de los datos para análisis comparativos entre países.
4.  **Exportación:** El sistema genera archivos procesados (`tuberculosis.csv`) tanto localmente como en la unidad de Drive para su uso posterior.

---

## 🚀 Cómo usar este repositorio
1. Abre el archivo `.ipynb` en este repositorio.
2. Haz clic en el botón **Open in Colab**.
3. Asegúrate de tener los archivos `population.csv` y `who.csv` en tu Google Drive dentro de una carpeta llamada `A/` para que las rutas coincidan:
   ```python
   # Ruta utilizada en el código
   pop = pd.read_csv("/content/drive/MyDrive/A/population.csv")

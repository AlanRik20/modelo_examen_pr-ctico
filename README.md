# Modelo de Parcial - TLP3

El objetivo de este trabajo fue realizar un análisis completo de un dataset con las calificaciones y asistencias de estudiantes, aplicando técnicas de limpieza, transformación, visualización y exportación de datos.

## Descripción general del proyecto

El análisis se llevó a cabo en un entorno virtual de Python mediante un Jupyter Notebook, y se estructuró en las siguientes etapas:

### 1.Importación del Dataset

Se utilizó la biblioteca **Pandas** para importar un archivo CSV con los datos originales.

### 3. Limpieza y Normalización de Datos

- Se normalizaron nombres de columnas para asegurar consistencia.
- Se convirtió la columna de **Asistencia** (que tenía valores como "75%", "101%") a datos numéricos reales.
- Se rellenaron valores nulos utilizando la mediana de cada columna.
- Se eliminaron registros o valores incoherentes.
- Se creó una nueva columna llamada `Promedio Estudiante` con el promedio entre `Parcial 1`, `Parcial 2` y `Final`.

### 4. Análisis Estadístico

- Se calcularon los promedios por **estudiante** y por **materia**.
- Se agruparon datos para obtener la **cantidad de aprobados** por materia.
- Se analizaron los niveles de asistencia por materia.

### 5. Visualización con Matplotlib

Se utilizaron gráficos para representar visualmente la información más relevante:

- Promedio general por estudiante
- Asistencia promedio por materia
- Cantidad de estudiantes aprobados por materia

### 6. Exportación del Dataset Limpio

Luego del procesamiento, el dataset limpio fue exportado a:

- Archivo `.CSV` actualizado
- Base de datos **SQLite** para facilitar consultas estructuradas

---

## Requisitos del entorno

Este proyecto fue desarrollado dentro de un **entorno virtual** de Python. Para poder ejecutarlo hay que hacer lo siguiente:

### Crear y activar entorno virtual

```bash
python -m venv env
# En Windows:
.\env\Scripts\activate
```

### Para instalar las dependencias:

```bash
pip install -r requirements.txt
```

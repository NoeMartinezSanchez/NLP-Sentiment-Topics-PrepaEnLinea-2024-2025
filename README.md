# Análisis de sentimiento y tópicos en comentarios de estudiantes (Prepa en Línea, 2024-2025)  

## 🔍 Resumen  
Proyecto de **Procesamiento de Lenguaje Natural (NLP)** que analiza comentarios de estudiantes hacia asesores virtuales de *Prepa en Línea* (datos 2024-2025). Mediante **BERT** (fine-tuning para español) y técnicas de modelado de tópicos, se identifican:  
- **Patrones de sentimiento** (clasificación binaria y multiclase).  
- **Temas críticos** (ej: claridad de materiales, comunicación con asesores).  
- **Recomendaciones basadas en datos** para la mejora pedagógica.  

## 🛠️ Tecnologías Clave  
- **Librerías NLP**: `transformers` (BERT), `spaCy` (procesamiento textual), `gensim` (LDA).  
- **Analítica**: Pandas, NumPy, Scikit-learn.  
- **Visualización**: Plotly (gráficos interactivos), WordCloud.  
- **Infraestructura**: Jupyter Notebooks, Google Colab (GPU para fine-tuning de BERT).  

## Procesamiento del texto

### Funciones clave:
limpiar_espacios()      # Normaliza espacios múltiples  
eliminar_puntuacion()   # Elimina signos de puntuación  
eliminar_stopwords()    # Filtra stopwords personalizadas (ej: "de", "que", "la")  

### Transformaciones aplicadas:
1. Lowercasing  
2. Reemplazo de guiones  
3. Eliminación de espacios redundantes  
4. Limpieza de puntuación  
5. Filtrado de 50+ stopwords en español  

## 📊 Métricas y Hallazgos

  

## 🎯 Impacto  
- **Decisiones pedagógicas**: Priorización de módulos con mayor insatisfacción.  
- **Gestión educativa**: Diseño de talleres para asesores basados en feedback negativo.  

## 📂 Estructura del Repositorio  

```python

data/
    ├── raw/                # Comentarios crudos (CSV)
    ├── processed/          # Datos unidos y limpios
notebooks/
    ├── Analisis tematico con limpieza antes (bueno).ipynb  # Realiza el analisis de sentimiento con BERT
    ├── Analitica comentarios AV 2024.ipynb  # Realiza la limpieza del texto, bigramas y trigramas de los datos del 2024.
    ├── Analitica comentarios AV 2025.ipynb  # Realiza la limpieza del texto, bigramas y trigramas de los datos del 2025.
images/                      # Contiene las imagenes del readme
Top-10-de-palabras-y-nube-de-palabras-(felicitaciones)/   # Contiene el top 10 de palabras por modulo nube de palabras
Top-10-de-palabras-y-nube-de-palabras-(sugerencias)/   # Contiene el top 10 de palabras por modulo nube de palabras

```

## 📌 Cómo Replicar el Análisis

1. Instalar dependencias: `pip install -r requirements.txt`.  
2. Ejecutar notebooks en orden numérico.  
3. Para fine-tuning de BERT: Usar GPU (Google Colab recomendado).  

---

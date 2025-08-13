# Análisis de sentimiento y tópicos en comentarios de estudiantes (Prepa en Línea, 2024-2025)  

## 🔍 Resumen  
Proyecto de **Procesamiento de Lenguaje Natural (NLP)** que analiza comentarios de estudiantes hacia asesores virtuales de *Prepa en Línea SEP* (datos 2024-2025). Mediante **BERT** (fine-tuning para español) y técnicas de modelado de tópicos, se identifican:  
- **Patrones de sentimiento** (clasificación binaria y multiclase).  
- **Temas críticos** (ej: claridad de materiales, comunicación con asesores).  
- **Recomendaciones basadas en datos** para la mejora pedagógica.  

## 🛠️ Tecnologías Clave  
- **Librerías NLP**: `transformers` (BERT), `spaCy` (procesamiento textual), `gensim` (LDA).  
- **Analítica**: Pandas, NumPy, Scikit-learn.  
- **Visualización**: Plotly (gráficos interactivos), WordCloud.  
- **Infraestructura**: Jupyter Notebooks, Google Colab (GPU para fine-tuning de BERT).  

## 📊 Métricas y Hallazgos  
1. **Distribución de sentimientos**:  
   - 65% positivos, 25% neutros, 10% negativos (2025 vs 60%/28%/12% en 2024).  
2. **Tópicos recurrentes**:  
   - "Retroalimentación oportuna" (módulo 3), "Dificultad en actividades" (módulo 5).  
3. **BERT vs Baselines**:  
   - **Accuracy de BERT**: 92% vs 85% (Random Forest con TF-IDF).  

## 🎯 Impacto  
- **Decisiones pedagógicas**: Priorización de módulos con mayor insatisfacción.  
- **Gestión educativa**: Diseño de talleres para asesores basados en feedback negativo.  

## 📂 Estructura del Repositorio  

data/
├── raw/ # Comentarios crudos (CSV/JSON)
├── processed/ # Datos limpios y vectorizados
notebooks/
├── 1_EDA.ipynb # Análisis exploratorio
├── 2_BERT_Sentiment.ipynb # Fine-tuning y evaluación
results/
├── dashboards/ # Gráficos interactivos
├── models/ # Modelos guardados (BERT, LDA)

## 📌 Cómo Replicar el Análisis  
1. Instalar dependencias: `pip install -r requirements.txt`.  
2. Ejecutar notebooks en orden numérico.  
3. Para fine-tuning de BERT: Usar GPU (Google Colab recomendado).  

---

### 💡 **Por qué Destacar BERT?**  
- **Precisión superior**: Modelo de transformers ajustado para español (ej: `dccuchile/bert-base-spanish-wwm`).  
- **Contexto lingüístico**: Captura ironía y negaciones (difícil con métodos clásicos como TF-IDF).  
- **Transfer Learning**: Aplicable a otros proyectos educativos en español.  

**Nota para reclutadores**: Si buscas detalles técnicos adicionales (hiperparámetros de BERT, métricas de evaluación), ¡avísame! Puedo ajustar el enfoque.  

--- 


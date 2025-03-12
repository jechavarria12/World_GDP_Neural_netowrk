# 🌍 Predicción de Categorías de PIB con Redes Neuronales

## 📝 Autores

- [*Mariana Solano Pineda*](https://www.linkedin.com/in/mariana-solano-pineda/)  
  Estudiante de economía y administración de empresas, Universidad de Los Andes  

- [*Ángela Aparicio*]()  
  Estudiante de economía, Universidad de Los Andes  

- [*Juan David Saldaña*](https://www.linkedin.com/in/juan-david-salda%C3%B1a-rivera-829ab62b3/)  
  Estudiante de economía, Universidad de Los Andes  

- [*Juan José Echavarría*]()  
  Estudiante de economía, Universidad de Los Andes  

- [*Juan Diego Barrios*]()  
  Estudiante de economía, Universidad de Los Andes  

---

## 📚 Descripción

Este proyecto utiliza redes neuronales para predecir la categoría del PIB de distintos países, transformando un problema de regresión en clasificación. Se entrenan y comparan distintos modelos para evaluar su desempeño en la predicción del PIB a partir de datos macroeconómicos.

---

## 🎯 Planteamiento del Problema

El objetivo es clasificar los países en tres categorías de PIB: **bajo**, **medio** y **alto**, a partir de sus datos históricos. Para ello, se emplean modelos de aprendizaje profundo con distintas arquitecturas y funciones de optimización.

---

## 📂 Contenido del Repositorio

- `main.ipynb` – Cuaderno principal con la implementación de modelos y análisis de resultados.  
- `README.md` – Este archivo con la descripción del proyecto y la relatoría.  
- `gdp_data.csv` – Datos históricos del PIB mundial.  
- `country_codes.csv` – Códigos de países utilizados en el análisis.  

---

## 🤖 Modelos Implementados

1. **Red Neuronal con Scikit-Learn** – Implementación básica con ajuste de hiperparámetros.  
2. **Red Neuronal Profunda con TensorFlow** – Modelo avanzado con múltiples capas ocultas.  
3. **Modelo con Mala Función de Pérdida** – Evaluación del impacto de una mala configuración y su corrección.  

---

## 📊 Evaluación de Modelos

Se analizan los modelos mediante:  
- Curvas de pérdida y precisión.  
- Matriz de confusión y métricas de clasificación.  
- Comparación de tasas de aprendizaje.  
- Curva ROC y análisis de importancia de variables.  

---

## 🚀 Requerimientos

- Python 3.x  
- Librerías: `numpy`, `pandas`, `scikit-learn`, `tensorflow`, `matplotlib`, `seaborn`, `shap`  

---

## 📄 Licencia

Este proyecto está bajo la Licencia MIT.  

---

## 📚 Relatoría del equipo

- **Preguntas que se hicieron y cómo resolvieron los problemas encontrados.**  
- **Soluciones y conclusiones a las que llegaron.**  
- **División del trabajo. En qué aportó cada integrante.**  

Juan José creó el repositorio de GitHub y lo compartió en un grupo de WhatsApp que creó Mariana para asegurar una comunicación efectiva. Decidimos organizar la división del trabajo para realizar el parcial. Juan José y Ángela comenzaron con la parte del código entre los dos, mientras que el resto del equipo (Mariana, Juan Diego y Juan David) se dedicó al análisis y a responder las preguntas, ya que hacer el código entre cinco personas nos pareció ineficiente.

Mariana propuso iniciar la descripción del README y la relatoría mientras Ángela y Juan José avanzaban con el código. Acordamos por unanimidad hacer el bono, y Juan David propuso buscar una base de datos que pudiera servir. Inicialmente, las bases de datos disponibles no cuadraban con los años requeridos para el parcial, por lo que Juan Diego ayudó a buscar alternativas. Aunque había problemas con las bases de datos, Sergio nos propuso enfocarnos en lo principal, dejando el bono como algo opcional. Finalmente, Juan David encontró bases adecuadas, lo que permitió completar el proyecto con éxito.

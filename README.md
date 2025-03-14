# 🌍 Predicción de Categorías de PIB con Redes Neuronales

📝 Autores

[*Mariana Solano Pineda*](https://www.linkedin.com/in/mariana-solano-pineda/)
Estudiante de economía y administración de empresas Universidad de Los Andes

[*Ángela Aparicio*]()
Estudiante de economía Universidad de Los Andes

[*Juan David Saldaña*]()
Estudiante de economía Universidad de Los Andes

[*Juan José Echavarría*]()
Estudiante de economía Universidad de Los Andes

[*Juan Diego Barrios*]()
Estudiante de economía Universidad de Los Andes

📚 Descripción

Este proyecto utiliza redes neuronales para predecir la categoría del PIB de distintos países, transformando un problema de regresión en clasificación. Se entrenan y comparan distintos modelos para evaluar su desempeño en la predicción del PIB a partir de datos macroeconómicos.

🎯 Planteamiento del Problema

El objetivo es clasificar los países en tres categorías de PIB: bajo, medio y alto, a partir de sus datos históricos. Para ello, se emplean modelos de aprendizaje profundo con distintas arquitecturas y funciones de optimización.

📂 Contenido del Repositorio
	•	main.ipynb – Cuaderno principal con la implementación de modelos y análisis de resultados.
	•	README.md – Este archivo con la descripción del proyecto y la relatoría
	•	gdp_data.csv – Datos históricos del PIB mundial.
	•	country_codes.csv – Códigos de países utilizados en el análisis.

🤖 Modelos Implementados
	1.	Red Neuronal con Scikit-Learn – Implementación básica con ajuste de hiperparámetros.
	2.	Red Neuronal Profunda con TensorFlow – Modelo avanzado con múltiples capas ocultas.
	3.	Modelo con Mala Función de Pérdida – Evaluación del impacto de una mala configuración y su corrección.

📊 Evaluación de Modelos

Se analizan los modelos mediante:
	•	Curvas de pérdida y precisión
	•	Matriz de confusión y métricas de clasificación
	•	Comparación de tasas de aprendizaje
	•	Curva ROC y análisis de importancia de variables

🚀 Requerimientos
	•	Python 3.x
	•	Librerías: numpy, pandas, scikit-learn, tensorflow, matplotlib, seaborn, shap

📄 Licencia

Este proyecto está bajo la Licencia MIT.

📚 Relatoría del equipo:

* Preguntas que se hicieron y cómo resolvieron los problemas encontrados.

* Soluciones y conclusiones a las que llegaron.

* División del trabajo. En qué aportó cada integrante.

Juan José creó el repositorio de GitHub y lo compartió en un grupo de WhatsApp que creó Mariana para asergurar una comunicación efectiva. Mientras tanto decidimos organizar la división para realizar el parcial. Juan José y Ángela decidieron comenzar a hacer la parte del código entre los dos y el resto (Mariana, Juan Diego y Juan David) decidieron hacer el análisis y las respuestas de las preguntas, debido a que hacer el código entre 5 nos pareció ineficiente. Mariana propuso comenzar a hacer la descripción del READMI y la relatoría, mientras había algo que analizar de lo que estaban haciendo Ángela y Juan José. Acordamos por unanimidad hacer el bono y Juan David propuso buscar una base de datos que había visto que consideraba que podía servir. Al ver que la base de datos no funionaba porque los años no cuadraban con la base de datos del parcial procedió a buscar una nueva con ayuda de Juan Diego. En la mayoría había problemas con los años, pero Sergio nos propuso concentrarnos en lo que no fuera del bono porque era más complejo. Juan David encontró luego varias bases de datos.

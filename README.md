# 🌍 Predicción de Categorías de PIB con Redes Neuronales

📝 Autores

[*Mariana Solano Pineda*](https://www.linkedin.com/in/mariana-solano-pineda/)
Estudiante de economía y administración de empresas Universidad de Los Andes

[*Ángela Aparicio*](www.linkedin.com/in/aparicio-angela)
Estudiante de economía Universidad de Los Andes

[*Juan David Saldaña Rivera*](https://www.linkedin.com/in/juan-david-salda%C3%B1a-rivera-829ab62b3/)
Estudiante de economía Universidad de Los Andes

[*Juan José Echavarría Villamizar*](www.linkedin.com/in/juan-jose-echavarria-villamizar)
Estudiante de economía Universidad de Los Andes

[*Juan Diego Barrios Esteban*](https://www.linkedin.com/in/juan-diego-barrios-esteban-6b684028b)
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

- **Miércoles 12/03/2025**

Juan José creó el repositorio de GitHub y lo compartió con el equipo a través de un grupo de WhatsApp, el cual había sido creado previamente por Mariana para asegurar una comunicación efectiva. En paralelo, se discutió la mejor manera de organizar la división del trabajo para la realización del parcial.

Se tomó la decisión de dividir el equipo en dos grupos:
**Grupo de programación:** Juan José y Ángela se ofrecieron para desarrollar la parte del código, ya que se consideró ineficiente que cinco personas trabajaran en ello simultáneamente.
**Grupo de análisis y redacción:** Mariana, Juan Diego y Juan David asumieron la tarea de analizar las preguntas y elaborar las respuestas, además de redactar el README y la relatoría. Mariana se encargó específicamente de la redacción del README y la relatoría, mientras esperaba los avances de Juan José y Ángela en la parte técnica.

Se acordó por unanimidad incluir el bono en el parcial. Juan David propuso una base de datos que había encontrado y que consideraba útil para el proyecto. Sin embargo, al intentar utilizarla, se identificó que los años no coincidían con los de la base de datos del parcial, lo que llevó a Juan David y Juan Diego a buscar nuevas alternativas. A pesar de que en varias bases se encontraron problemas similares con los años, Sergio sugirió que, por el momento, el equipo se enfocara en las preguntas principales del parcial y dejara el bono para después.

Finalmente, Juan David encontró varias bases de datos que compartió en el grupo para futuras referencias. Para el final de la clase, Juan José y Ángela ya habían avanzado en el procesamiento de los datos, aunque aún quedaban pendientes algunos detalles. En paralelo, Mariana había terminado la descripción del README y la parte inicial de la relatoría, mientras que Juan Diego y Juan David revisaron las instrucciones del parcial y analizaron las preguntas sin responderlas aún. 

Se acordó organizar más tarde ese día para definir cómo finalizar el parcial, ya que en la sesión del viernes no habría suficiente tiempo para completarlo. Por la tarde acordamos que el jueves se terminaría la parte del código y el análisis, para que el viernes se pudiera resolver cualquier duda restante. Se acordó que el grupo de análisis y redacción se reuniera el jueves en la noche a las 19h para hacer el análisis, luego de que el grupo de programación terminara el código.

- **Jueves 13/03/2025**

Al día siguiente varios integrantes salieron de parciales, por lo que hubo más tiempo para continuar con el parcial. A lo largo del día, el equipo continuó avanzando en el desarrollo del parcial, asegurándose de que cada miembro comprendiera su rol dentro del proyecto y resolviendo dudas conforme surgían. Se mantuvo una comunicación constante a través del grupo de WhatsApp para coordinar los avances y resolver cualquier inconveniente de manera ágil. Ángela se reunió con Sergio a las 14h para revisar **algo que faltaba del procesamiento de datos** que había continuado Juan José y en la tarde noche le compartió al equipo una versión preliminar del script con el procesamiento de datos ya revisado por Sergio mientras Juan José continuaba trabajando en los modelos. A las 19h30 Juan Diego, Juan David y Mariana se reunieron para continuar con el análisis de las preguntas. Sin embargo, al revisar el script que estaban desarrollando Juan José y Ángela, se encontraron con dificultades para comprender la nomenclatura de la variable del PIB, la cual era clave para clasificar los datos y responder algunas preguntas del parcial. Para resolver esta situación, el grupo decidió contactar a Ángela, quien explicó la lógica detrás del procesamiento de datos que habían implementado. Gracias a su explicación, el equipo pudo continuar con el análisis de manera más eficiente y responder las preguntas de manera fundamentada. Solo hizo falta una de las preguntas, que tenía que ver con la correlación entre los datos, puesto que el bloque de código

from ydata_profiling import ProfileReport
reporte_train = ProfileReport(X_train, title="Profiling Report Train dataset")
reporte_train.to_file("reporte_train.html")
reporte_train

no corrió en ninguno de los computadores del equipo de análisis (esto debido a la capacidad del RAM), pero Juan José sí era capaz de visualizarlo. El equipo le comentó la situación a Juan José, quien les propuso mostrarles la terminal de ese bloque de código para que pudieran hacer el análisis. El equipo de análisis respondió las preguntas del parcial combinando su conocimiento previo, la información obtenida del código desarrollado y herramientas de inteligencia artificial como DeepSeek y ChatGPT para validar y complementar sus respuestas. Por ejemplo, al abordar la pregunta sobre los desafíos de una serie de tiempo, inicialmente analizaron la problemática basándose en lo aprendido en clase. Sin embargo, al contrastar su respuesta con la IA, descubrieron que omitían factores clave como la estacionalidad, la autocorrelación y el sesgo en los datos. Esta verificación les permitió ajustar y enriquecer su análisis, asegurando una respuesta más precisa y fundamentada.Ángela y Juan José se reunireron con Sergio a las 22h para terminar la parte de los modelos y poderlo enviar al grupo para añadir al documento de Google Colab las preguntas que se habían respondido en la reunión.

- **Viernes 14/03/2025**

Temprano en la mañana Juan José subió la versión final del documento de Colab, donde ya estaba el código terminado mientras que Mariana continuaba con la relatoría. Añadió al documento las preguntas respondidas el día anterior y arregló un poco la interfaz del documento. En la clase, a las 11h el equipo de análisis revisó detalles finales de las preguntas que faltaban y, de igual forma, Mariana terminó la relatoría.

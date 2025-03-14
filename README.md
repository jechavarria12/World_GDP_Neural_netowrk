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

Al día siguiente varios integrantes salieron de parciales, por lo que hubo más tiempo para continuar con el parcial. A lo largo del día, el equipo continuó avanzando en el desarrollo del parcial, asegurándose de que cada miembro comprendiera su rol dentro del proyecto y resolviendo dudas conforme surgían. Se mantuvo una comunicación constante a través del grupo de WhatsApp para coordinar los avances y resolver cualquier inconveniente de manera ágil. Ángela se reunió con Sergio a las 14h para arreglar una parte del procesamiento del script que había creado Juan José, ya que era esencial incluir el nombre de los países, sacarle el promedio a cada año del PIB para otorgarle un número y también asignarle un valor categórico a las regiones de 1 a 6. En la tarde noche Ángela le compartió al equipo una versión preliminar del script con el procesamiento de datos ya revisado por Sergio mientras Juan José continuaba trabajando en los modelos. A las 19h30 Juan Diego, Juan David y Mariana se reunieron para continuar con el análisis de las preguntas. Sin embargo, al revisar el script que estaban desarrollando Juan José y Ángela, se encontraron con dificultades para comprender la nomenclatura de la variable del PIB, la cual era clave para clasificar los datos y responder algunas preguntas del parcial. Para resolver esta situación, el grupo decidió contactar a Ángela, quien explicó la lógica detrás del procesamiento de datos que habían implementado. Gracias a su explicación, el equipo pudo continuar con el análisis de manera más eficiente y responder las preguntas de manera fundamentada. Solo hizo falta una de las preguntas, que tenía que ver con la correlación entre los datos, puesto que el bloque de código.

from ydata_profiling import ProfileReport
reporte_train = ProfileReport(X_train, title="Profiling Report Train dataset")
reporte_train.to_file("reporte_train.html")
reporte_train

no corrió en ninguno de los computadores del equipo de análisis, pero Juan José sí era capaz de visualizarlo. El equipo le comentó la situación a Juan José, quien les propuso mostrarles los resultados de ese bloque de código para que pudieran hacer el análisis de la correlación. Luego el viernes el equipo de análisis se dio cuenta de que sí le corría, solo que no habían visto dónde se descargaba el reporte del profiling, que era el documento esencial para hacer el análisis. El equipo de análisis respondió las preguntas del parcial combinando su conocimiento previo, la información obtenida del código desarrollado y herramientas de inteligencia artificial como DeepSeek y ChatGPT para validar y complementar sus respuestas. Por ejemplo, al abordar la pregunta sobre los desafíos de una serie de tiempo, inicialmente analizaron la problemática basándose en lo aprendido en clase. Sin embargo, al contrastar su respuesta con la IA, descubrieron que omitían factores clave como la estacionalidad, la autocorrelación y el sesgo en los datos. Esta verificación les permitió ajustar y enriquecer su análisis, asegurando una respuesta más precisa y fundamentada. Ángela y Juan José se reunireron con Sergio a las 22h y otros grupos para terminar la parte de los modelos y poderlo enviar al resto para añadir al documento de Google Colab las preguntas que se habían respondido en la reunión. Juan José enfrentó varios desafíos al entrenar los modelos de redes neuronales, especialmente para las redes neuronales profundas, al definir los parámetros clave como la estructura de las capas, el número de neuronas por capa, la tasa de dropout, los learning rates, el número de épocas y el batch size. En primer lugar, la variable y era categórica, pero el modelo no la aceptaba en ese formato, por lo que tuvo que convertirla a valores numéricos, un proceso que resultó complejo. Luego, al establecer la capa de salida con tres neuronas, fue necesario aplicar OneHotEncoder para representar correctamente las clases. Además, inicialmente utilizó una función de pérdida incorrecta, cuando en realidad debía emplear una función de pérdida categórica, pero al final se dio cuenta y pudo solucionar la situación. Finalmente, tuvo que ajustar la función de activación para que fuera compatible con la función de pérdida, asegurando así un entrenamiento adecuado del modelo.

- **Viernes 14/03/2025**

Temprano en la mañana Juan José envió la versión final del documento de Colab, donde ya estaba el código terminado mientras que Mariana continuaba con la relatoría. Añadió al documento las preguntas respondidas el día anterior y arregló un poco la interfaz del documento. En la clase, a las 11h el equipo de análisis se dio cuenta de que había otras preguntas que todavía había que contestar, por lo que Juan David procedió a revisarlas mientras que Mariana y Juan Diego terminaban de responder las que quedaban del día anterior. En ese momento fue cuando se dieron cuenta de que no sabían cómo descargar el reporte de estadísticas descriptivas y Juan José les ayudó. Ya con esto resuleto fue posible terminar de responder las preguntas restantes. Mientras tanto, Juan José, con ayuda de Juan David, completaron un bono para aumentar la nota. Así es como terminaron de hacer el bono, subieron el documento de nuevo al GitHub para que el equipo de análisis pudiera añadir las preguntas al documento, subir a Bloque Neón el parcial y darlo por finalizado.

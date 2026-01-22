# FITBOT - AI Deep Learning Chatbot 🤖🏋️‍♂️

**FITBOT** es un asistente virtual de fitness inteligente que utiliza una **Red Neuronal Secuencial** entrenada localmente. A diferencia de los chatbots basados en reglas simples o APIs externas, FitBot emplea técnicas de **Deep Learning** y **Procesamiento de Lenguaje Natural (NLP)** para clasificar las intenciones del usuario y ofrecer respuestas precisas sobre rutinas de ejercicio, nutrición y salud.

---

## ✨ Características Principales

* **Modelo de Red Neuronal:** Entrenado con **TensorFlow** y **Keras** para lograr una clasificación de intenciones de alta precisión.
* **Procesamiento de Texto (NLP):** Implementa la librería **NLTK** para la tokenización y lematización (reducción de palabras a su raíz lógica).
* **Entrenamiento Local:** No depende de servicios de terceros, lo que garantiza privacidad, baja latencia y funcionamiento offline.
* **Sistema de Intenciones (Intents):** Estructura basada en el archivo `intents.json`, lo que permite expandir el conocimiento del bot sin modificar el código base.
* **Historial de Conversación:** Almacena registros de interacciones en un archivo JSON para el seguimiento de la experiencia del usuario.

---

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Python 3.x
* **Inteligencia Artificial:** TensorFlow, Keras
* **NLP:** NLTK (Natural Language Toolkit)
* **Data Management:** NumPy, Pickle (serialización), JSON

---

## 📂 Estructura del Proyecto (Directorio FITBOT)

Basado en la arquitectura del repositorio:

* **`training.py`**: Script responsable de pre-procesar los datos de `intents.json`, construir la arquitectura de la red neuronal y realizar el entrenamiento.
* **`chatbot.py`**: Script principal de ejecución que carga el modelo entrenado y gestiona la lógica de respuesta en tiempo real.
* **`intents.json`**: El conjunto de datos (dataset) que define los patrones de entrada del usuario y las respuestas correspondientes.
* **`chatbot_model.h5`**: El modelo de red neuronal exportado, listo para su uso inmediato.
* **`words.pkl` / `classes.pkl`**: Archivos binarios que guardan el vocabulario y las etiquetas clasificadas generadas durante el entrenamiento.
* **`conversation_history.json`**: Archivo de log que registra el flujo de los chats realizados.
* **`static/`**: Carpeta de recursos estáticos para la interfaz de usuario.

---

## 🚀 Instalación y Uso

### 1. Requisitos previos
Es necesario tener instalado Python 3.x y las dependencias de Machine Learning:
```bash
pip install tensorflow nltk numpy
2. Entrenamiento del Bot
Si decides modificar o añadir nuevas preguntas/respuestas en intents.json, debes regenerar el modelo:

Bash

python training.py
3. Ejecución del Chatbot
Para iniciar el asistente y comenzar la conversación:

Bash

python chatbot.py
✒️ Autor
Jose Martínez Silva - JoseMartinezS

📄 Licencia
Este proyecto está bajo la Licencia MIT. Puedes usarlo, mejorarlo y distribuirlo libremente para fines educativos o de desarrollo profesional en el área de salud y fitness.

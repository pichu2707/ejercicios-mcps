# Ejercicio Multiagente con Google ADK y Herramientas Python

## Descripción

Este proyecto es un ejemplo práctico de cómo construir un sistema multiagente utilizando [Google ADK (Agent Development Kit)](https://google.github.io/adk-docs/) y herramientas personalizadas en Python. El objetivo es simular un flujo de trabajo de e-commerce donde diferentes agentes colaboran para gestionar productos, carrito de compras y cálculos matemáticos, integrando lógica de negocio y capacidades de IA generativa.

Una modificación del código de [Carlos Alarcón](https://www.youtube.com/@alarcon7a) para hacer de este un código más dinámico, encontrando diferentes problemas como la realización de los cálculos del agente a través del Chat
## Características principales

- **Multiagente por diseño:**  
  El sistema cuenta con agentes especializados (por ejemplo, agente de e-commerce y agente calculadora) que colaboran entre sí.
- **Herramientas Python integradas:**  
  Todas las operaciones matemáticas y de negocio (sumas, porcentajes, gestión de carrito, búsqueda de productos) se realizan mediante funciones Python, garantizando precisión y control.
- **Orquestación flexible:**  
  Los agentes pueden delegar tareas entre sí y utilizar herramientas según el contexto de la conversación.
- **Interfaz conversacional:**  
  Incluye una interfaz de chat (Gradio) donde el usuario puede interactuar con el sistema de manera natural.
- **Uso de modelos LLM:**  
  El sistema puede trabajar tanto con modelos de Google Gemini como con modelos de OpenAI, según la configuración.

## Estructura del proyecto

- `ejercicio_clase_2.ipynb`: Notebook principal con todo el código, definición de agentes, herramientas y la interfaz de chat.
- `requirements.txt`: Dependencias necesarias para ejecutar el proyecto.
- `.env.example`: Ejemplo de archivo de variables de entorno para claves API.
- `README.md`: Este archivo.

## Instalación

1. **Clona el repositorio o descarga los archivos.**
2. **Instala las dependencias:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Configura tus claves API**  
   Crea un archivo `.env` en la raíz del proyecto y añade tus claves:
   ```
   OPENAI_API_KEY=tu_clave_openai
   GEMINI_API_KEY=tu_clave_gemini
   ```

## Ejecución

Abre el notebook `ejercicio_clase_2.ipynb` en VS Code o Jupyter y ejecuta las celdas.  
Al final, se lanzará una interfaz de chat donde puedes interactuar con el sistema.

## Ejemplo de uso

- **Buscar productos:**  
  “¿Tienes mesas blancas de comedor?”
- **Agregar al carrito:**  
  “Añade 2 sillas de comedor gris al carrito.”
- **Cálculos matemáticos:**  
  “¿Cuánto es el 15% de 200?”  
  “¿Cuál es el precio total del carrito?”

El sistema usará siempre las funciones Python para los cálculos, garantizando respuestas correctas y fiables.

## Créditos

Ejercicio desarrollado para la clase de MCP (Multiagent Conversational Programming).  
Autor: Javi Lázaro
email: [hola@javilazaro.es](mailto:hola@javilazaro.es)
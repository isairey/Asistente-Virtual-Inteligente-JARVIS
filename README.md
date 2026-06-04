# 🤖 JARVIS - Asistente Virtual Inteligente

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python)
![Status](https://img.shields.io/badge/Estado-Activo-success?style=for-the-badge)
![License](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge)

## 📌 Descripción

**JARVIS (Just a Rather Very Intelligent System)** es un asistente virtual desarrollado en Python inspirado en el famoso sistema de inteligencia artificial mostrado en las películas de Iron Man.

Este proyecto permite automatizar diversas tareas diarias mediante comandos de voz, ofreciendo una experiencia interactiva capaz de controlar aplicaciones, consultar información en línea, reproducir contenido multimedia y ejecutar múltiples funciones del sistema operativo.

---

## 🚀 Características Principales

### 🗣️ Interacción por Voz
- Saluda al usuario.
- Reconoce comandos de voz.
- Responde mediante síntesis de voz.

### 📅 Información General
- Consulta fecha y hora actual.
- Obtiene información meteorológica de cualquier ciudad.
- Muestra noticias destacadas.
- Consulta información de personas mediante Wikipedia.
- Responde preguntas generales usando WolframAlpha.

### 🌐 Navegación Web
- Abre cualquier sitio web.
- Realiza búsquedas en Google.
- Reproduce videos y música desde YouTube.

### 💻 Control del Sistema
- Abre aplicaciones instaladas.
- Cambia entre ventanas activas.
- Captura pantallas con nombres personalizados.
- Obtiene información del sistema:
  - Uso de CPU
  - Uso de memoria RAM
  - Estado de batería
- Muestra la dirección IP pública.

### 📍 Ubicación y Mapas
- Busca ubicaciones.
- Calcula distancias entre lugares.
- Abre ubicaciones directamente en mapas.

### 📧 Productividad
- Envía correos electrónicos.
- Guarda notas importantes.
- Consulta eventos próximos desde Google Calendar.

### 🎵 Entretenimiento
- Reproduce música.
- Cuenta chistes aleatorios.
- Reproduce canciones desde YouTube.

### 🧮 Herramientas Inteligentes
- Resuelve expresiones matemáticas.
- Realiza cálculos complejos.
- Responde preguntas mediante WolframAlpha.

### 🎨 Interfaz Gráfica
- Incluye una interfaz gráfica amigable.
- Diseño modular y personalizable.

---


## 🛠️ Tecnologías Utilizadas

- Python 3.8+
- PyQt5
- SpeechRecognition
- PyAudio
- pyttsx3
- Wikipedia API
- OpenWeatherMap API
- WolframAlpha API
- Google Calendar API
- Selenium
- Requests

---

## 🔑 APIs Necesarias

Para ejecutar correctamente el proyecto es necesario obtener las siguientes claves API:

### OpenWeatherMap
Permite consultar información meteorológica.

https://openweathermap.org/api

### WolframAlpha
Permite responder preguntas y resolver operaciones matemáticas.

https://www.wolframalpha.com/

### Google Calendar API
Permite consultar eventos del calendario.

https://developers.google.com/calendar/auth

---

## ⚙️ Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/isairey/Asistente-Virtual-Inteligente-JARVIS.git
cd Asistente-Virtual-Inteligente-JARVIS
```

### 2. Crear el archivo de configuración

Crear un archivo llamado:

```python
config.py
```

Con el siguiente contenido:

```python
weather_api_key = "TU_API_KEY"

email = "TU_CORREO"

email_password = "TU_CONTRASEÑA"

wolframalpha_id = "TU_WOLFRAM_ID"
```

Copiar el archivo dentro de:

```bash
Jarvis/config/
```

### 3. Crear entorno virtual

Con Anaconda:

```bash
conda create -n jarvis python=3.8.5
```

Activar entorno:

```bash
conda activate jarvis
```

O con venv:

```bash
python -m venv venv
```

Activar:

```bash
# Windows
venv\Scripts\activate

# Linux / Mac
source venv/bin/activate
```

### 4. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 5. Instalar PyAudio

En Windows puede requerirse instalación manual mediante wheel.

```bash
pip install PyAudio
```

Si presenta errores, instalar mediante archivo `.whl`.

### 6. Ejecutar la aplicación

```bash
python main.py
```

---

## 📂 Estructura del Proyecto

```text
JARVIS
│
├── driver/
│
├── Jarvis/
│   ├── config/
│   │   └── APIs y configuraciones
│   │
│   ├── features/
│   │   └── Funcionalidades del asistente
│   │
│   └── utils/
│       └── Recursos gráficos
│
├── __init__.py
├── gui.ui
├── main.py
└── requirements.txt
```

---

## ➕ Agregar Nuevas Funcionalidades

El proyecto es completamente modular.

Para agregar una nueva característica:

### Paso 1
Crear un nuevo archivo dentro de:

```bash
Jarvis/features/
```

### Paso 2
Implementar la función correspondiente.

### Paso 3
Importar la función en:

```python
__init__.py
```

### Paso 4
Agregar los comandos de voz que activarán dicha función.

---

## 📈 Posibles Mejoras Futuras

- Integración con modelos de Inteligencia Artificial modernos.
- Conversaciones más naturales mediante NLP.
- Mejora de la interfaz gráfica.
- Compatibilidad multiplataforma avanzada.
- Integración con dispositivos IoT.
- Automatización doméstica.
- Reconocimiento facial.
- Sistema de aprendizaje personalizado.

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas.

Si deseas colaborar:

1. Haz un Fork del proyecto.
2. Crea una rama para tu funcionalidad.
3. Realiza los cambios.
4. Envía un Pull Request.

---

## 📜 Licencia

Este proyecto está distribuido bajo la licencia MIT.

Desarrollado originalmente por Atharva Ingle.

---

## 👨‍💻 Autor

Proyecto inspirado en el asistente J.A.R.V.I.S. de Iron Man.

Adaptado y mejorado para fines educativos y de automatización personal utilizando Python.

# FamiliaBot 👨‍👩‍👧‍👦

![Logo de FamiliaBot](https://github.com/bladealex9848/FamiliaBot/blob/main/assets/logo.jpg)

[![Version](https://img.shields.io/badge/versión-1.0.0-darkgreen.svg)](https://github.com/bladealex9848/FamiliaBot)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30.0-ff4b4b.svg)](https://streamlit.io/)
[![OpenAI](https://img.shields.io/badge/OpenAI_API-v2-00C244.svg)](https://platform.openai.com/)
[![Licencia](https://img.shields.io/badge/Licencia-MIT-yellow.svg)](LICENSE)
[![Visitantes](https://api.visitorbadge.io/api/visitors?path=https%3A%2F%2Ffamiliabot.streamlit.app&label=Visitantes&labelColor=%235d5d5d&countColor=%231e7ebf&style=flat)](https://familiabot.streamlit.app)

## ⚖️ Descripción

FamiliaBot es un asistente virtual especializado en derecho de familia en Colombia, desarrollado con Streamlit y la API de OpenAI. Su base de conocimiento incluye el Código Civil Colombiano, la Ley 1564 de 2012 (Código General del Proceso), la Ley 1098 de 2006 (Código de la Infancia y la Adolescencia), la Ley 2388 de 2024, jurisprudencia relevante de la Corte Suprema de Justicia, y la Ley 1996 de 2019.

Este asistente está diseñado para proporcionar información clara y accesible sobre temas de derecho de familia a estudiantes, profesionales del derecho y ciudadanos que necesiten orientación en este ámbito jurídico.

## 🔍 Funcionalidades Principales

### 1. Información Jurídica Especializada
- **Tipos de Familia**: Explicación sobre los diferentes modelos familiares reconocidos en Colombia
- **Matrimonio y Divorcio**: Información sobre requisitos, efectos legales y procedimientos
- **Uniones Maritales de Hecho**: Requisitos para su reconocimiento y efectos jurídicos
- **Régimen Patrimonial**: Sociedad conyugal, capitulaciones matrimoniales y liquidación de bienes

### 2. Aspectos Relacionados con Menores
- **Custodia y Cuidado Personal**: Información sobre los diferentes tipos de custodia
- **Régimen de Visitas**: Explicación sobre cómo se establece y modifica
- **Obligaciones Alimentarias**: Quiénes están obligados, cómo se fijan y procedimientos de reclamación
- **Patria Potestad**: Derechos y obligaciones de los padres respecto a sus hijos

### 3. Procesos Judiciales Familiares
- **Procesos de Familia**: Información sobre competencia y jurisdicción
- **Medidas de Protección**: Procedimientos ante violencia intrafamiliar
- **Trámites Administrativos**: Procesos ante comisarías de familia y defensorías
- **Conciliación en Familia**: Requisitos y efectos de los acuerdos conciliatorios

### 4. Análisis de Documentos
- **Procesamiento OCR**: Análisis de documentos legales mediante tecnología avanzada
- **Evaluación Jurídica**: Análisis preliminar de documentos desde la perspectiva del derecho de familia
- **Identificación de Elementos Clave**: Detección de aspectos relevantes en documentos legales
- **Sugerencias Normativas**: Referencias a leyes y jurisprudencia aplicables

## 🚀 Instalación

### Requisitos Previos
- Python 3.8 o superior
- Pip (administrador de paquetes de Python)
- Cuenta en OpenAI con acceso a la API
- Cuenta en Mistral AI con acceso a la API (para OCR)
- Asistente FamiliaBot configurado en OpenAI

### Pasos de Instalación

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/bladealex9848/FamiliaBot.git
   cd FamiliaBot
   ```

2. **Crear un entorno virtual (recomendado)**
   ```bash
   python -m venv venv
   
   # En Windows
   venv\Scripts\activate
   
   # En macOS/Linux
   source venv/bin/activate
   ```

3. **Instalar las dependencias**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configurar credenciales**

   **Opción A: Usando variables de entorno**
   ```bash
   # En Windows
   set OPENAI_API_KEY=tu-api-key-aqui
   set MISTRAL_API_KEY=tu-api-key-mistral-aqui
   set ASSISTANT_ID=tu-assistant-id-aqui
   
   # En macOS/Linux
   export OPENAI_API_KEY=tu-api-key-aqui
   export MISTRAL_API_KEY=tu-api-key-mistral-aqui
   export ASSISTANT_ID=tu-assistant-id-aqui
   ```

   **Opción B: Usando archivo secrets.toml**
   
   Crea un archivo `.streamlit/secrets.toml` con el siguiente contenido:
   ```toml
   OPENAI_API_KEY = "tu-api-key-aqui"
   MISTRAL_API_KEY = "tu-api-key-mistral-aqui"
   ASSISTANT_ID = "tu-assistant-id-aqui"
   ```

## ⚙️ Uso

### Iniciar la Aplicación

```bash
streamlit run app.py
```

Esto lanzará la aplicación y abrirá automáticamente una ventana del navegador en `http://localhost:8501`.

### Funcionalidades del Asistente

1. **Consultas sobre Derecho de Familia**
   - Pregunta sobre conceptos jurídicos, requisitos legales o procedimientos
   - Ejemplo: "¿Cuáles son los requisitos para solicitar el divorcio en Colombia?"

2. **Información sobre Procesos Judiciales**
   - Consulta trámites, competencias y jurisdicción en asuntos de familia
   - Ejemplo: "¿Qué juez es competente para conocer una demanda de alimentos?"

3. **Consultas sobre Menores**
   - Obtén información sobre custodia, alimentos, régimen de visitas y patria potestad
   - Ejemplo: "¿Cómo se establece la custodia compartida en Colombia?"

4. **Análisis de Documentos**
   - Sube documentos para recibir un análisis desde la perspectiva del derecho de familia
   - El asistente puede procesar sentencias, demandas, acuerdos o contratos

5. **Referencia Normativa**
   - Solicita información sobre leyes específicas o jurisprudencia relevante
   - Ejemplo: "¿Qué establece la Ley 1098 de 2006 sobre el derecho de alimentos?"

## ⚠️ Limitaciones

- FamiliaBot proporciona información general y no constituye asesoramiento legal personalizado
- La información se basa en el conocimiento disponible hasta octubre de 2023
- Para casos específicos, siempre es recomendable consultar con un abogado especializado
- El análisis de documentos es preliminar y no reemplaza la revisión profesional

## 📊 Escenarios de Uso

### 1. Estudiantes de Derecho
- Consulta de conceptos y normativa sobre derecho de familia
- Preparación para exámenes y trabajos académicos
- Comprensión de procedimientos judiciales

### 2. Profesionales del Derecho
- Referencia rápida sobre normativa y jurisprudencia
- Análisis preliminar de documentos
- Actualización sobre interpretaciones jurídicas

### 3. Ciudadanos en General
- Orientación básica sobre derechos y deberes familiares
- Comprensión de procesos antes de acudir a un profesional
- Información sobre trámites y procedimientos

## 👥 Contribuciones

Las contribuciones son bienvenidas. Para contribuir al desarrollo de FamiliaBot:

1. Realiza un fork del repositorio
2. Crea una nueva rama (`git checkout -b feature/nueva-funcionalidad`)
3. Implementa tus cambios
4. Envía un pull request

## 📝 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.

## 🙏 Agradecimientos

- **OpenAI** por proporcionar la tecnología que impulsa el asistente
- **Mistral AI** por la tecnología OCR utilizada en el procesamiento de documentos
- **Streamlit** por facilitar el desarrollo de interfaces intuitivas
- **Comunidad jurídica colombiana** por su contribución al derecho de familia

## 👤 Autor

Creado con ❤️ por [Alexander Oviedo Fadul](https://github.com/bladealex9848)

[GitHub](https://github.com/bladealex9848) | [Website](https://alexanderoviedofadul.dev) | [LinkedIn](https://www.linkedin.com/in/alexander-oviedo-fadul/) | [Instagram](https://www.instagram.com/alexander.oviedo.fadul) | [Twitter](https://twitter.com/alexanderofadul) | [Facebook](https://www.facebook.com/alexanderof/) | [WhatsApp](https://api.whatsapp.com/send?phone=573015930519&text=Hola%20!Quiero%20conversar%20contigo!%20)

---

## 💼 Mensaje Final

FamiliaBot busca democratizar el acceso a la información sobre derecho de familia en Colombia, facilitando la comprensión de conceptos jurídicos complejos. Aunque este asistente proporciona información valiosa, recuerda que cada situación familiar es única y puede requerir orientación profesional personalizada.

*"El conocimiento de tus derechos y obligaciones familiares es el primer paso para tomar decisiones informadas y proteger lo más valioso: tu familia."*
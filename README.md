📊 Optimización e Inteligencia de Datos en Seguimiento de Proyectos
📌 Descripción del Proyecto
Sistema integral de gobernanza y analítica de datos diseñado para transformar un seguimiento tradicional de proyectos (Project Tracker) en un modelo auditado con detección automática de alertas mediante Python, informes ejecutivos impulsados por IA (Gemini API).
🎯 Problema de Negocio
•	Lentitud en reportes: Ineficiencia y consumo excesivo de tiempo en la preparación manual de informes de riesgo para comités directivos.
•	Falta de visibilidad: Inconsistencia en el seguimiento manual de hitos, fechas y dependencias críticas.
•	Calidad de datos: Presencia de registros incompletos o desactualizados en los avances del proyecto.
🛠️ Arquitectura y Tecnologías
•	Python (Pandas, OpenPyXL): Limpieza, transformación de datos y motor de reglas de auditoría.
•	Google GenAI SDK (Gemini API): Automatización de informes ejecutivos de gobernanza en formato HTML.
•	Excel: Almacenamiento estructurado de tracker de tareas y minutas.
🔄 Flujo de Trabajo (End-to-End Pipeline)
1.	Ingesta y Auditoría Automática (Python):
Procesamiento del archivo Project_Tracker.xlsx para aplicar 5 reglas clave de gestión (atrasos activos, desviaciones históricas, bloqueos por dependencia, calidad de datos y tareas críticas sin iniciar). Generación del archivo auditado Project_Tracker_Audited.xlsx.
2.	Generación de Reportes con IA Generativa (Gemini API):
Consumo automatizado del dataset auditado usando la librería oficial google-genai para estructurar un informe gerencial en código HTML moderno y estilizado (Informe_Ejecutivo_Gobernanza.html).
🚀 Cómo Ejecutar este Proyecto
1. Prerrequisitos
Instala las librerías necesarias ejecutando en la terminal:
Bash
pip install pandas openpyxl google-genai
2. Configuración de Variables de Entorno
Configura tu API Key de Google AI Studio:
En Windows (CMD):
DOS
set GEMINI_API_KEY="tu_api_key_aqui"
En Linux / macOS:
Bash
export GEMINI_API_KEY="tu_api_key_aqui"
3. Ejecución de Scripts
a.	Ejecutar el motor de auditoría:
Bash
python auditoria_tracker.py
b.	Generar el informe HTML con IA:
Bash
python generar_informe_html.py
📂 Estructura del Repositorio
Plaintext
├── Project_Tracker.xlsx
├── Project_Tracker_Audited.xlsx
├── auditoria_tracker.py
├── generar_informe_html.py
├── Informe_Ejecutivo_Gobernanza.html
└── README.md
👤 Autor
Alcira | Data & Governance Analyst
GitHub Profile


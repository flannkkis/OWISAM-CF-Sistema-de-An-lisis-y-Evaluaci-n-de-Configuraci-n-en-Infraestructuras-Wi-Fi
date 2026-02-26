OWISAM-CF
Sistema de Análisis y Evaluación de Configuración en Infraestructuras Wi-Fi


- Descripción
OWISAM-CF es una herramienta desarrollada en Python para analizar configuraciones de redes Wi-Fi y detectar posibles debilidades de seguridad.
El sistema escanea redes inalámbricas cercanas, recopila parámetros técnicos relevantes y aplica un conjunto de reglas basadas en buenas prácticas de seguridad para identificar configuraciones potencialmente inseguras.
El objetivo no es realizar ataques, sino evaluar configuraciones y generar un informe de riesgos.

- Objetivos del Proyecto
Detectar redes Wi-Fi abiertas (sin cifrado).
Identificar el uso de cifrados obsoletos como WEP o WPA.
Detectar SSID por defecto basados en patrones comunes.
Analizar la distribución de canales y detectar posibles saturaciones.
Clasificar redes según nivel de riesgo (Bajo, Medio, Alto).
Generar un reporte automático con recomendaciones de mejora.

- Funcionamiento General
El sistema se divide en tres fases principales:

 1️. Escaneo
Se recopila información básica de redes Wi-Fi cercanas:
SSID
BSSID
Canal
Tipo de cifrado
Nivel de señal

2. Análisis
Se aplican reglas de evaluación como:
Red abierta → Riesgo alto
WEP o WPA → Riesgo medio/alto
SSID por defecto → Advertencia
Canal saturado (ej. canal 6 en 2.4 GHz) → Advertencia

4. Generación de Reporte
El sistema genera:
Resumen general
Lista de redes detectadas
Clasificación por nivel de riesgo
Recomendaciones de seguridad

- Estructura del Proyecto
OWISAM-CF

 ├── scanner.py
 
 ├── analyzer.py
 
 ├── report.py
 
 ├── main.py
 
 ├── utils.py
 
 ├── README.md
 
 └── requirements.txt

- Tecnologías Utilizadas
Python 3.15
Librerías de captura y análisis de redes inalámbricas
Generación de reportes en formato texto o JSON
Criterios de Evaluación de Riesgo
Configuración Detectada	Nivel de Riesgo
Red abierta	Alto
WEP	Alto
WPA	Medio
SSID por defecto	Advertencia
Canal saturado	Advertencia

- Instalación
Rellenar

- Uso
Rellenar

- Buenas Prácticas Consideradas
Rellenar

- Advertencia Legal
Esta herramienta está diseñada exclusivamente con fines educativos y de análisis en entornos controlados o redes propias. No debe utilizarse para auditar redes sin autorización.

- Autor
Proyecto desarrollado como TFM del Curso de Especialización en Ciberseguridad en los Entornos de las Tecnologías de la Información realizado por Alejandro Flanagan

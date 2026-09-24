# Entrega-Final-Gomez-Matias-Com97415
Automatización de comunicados impositivos y de compliance con n8n, Google Gemini y Notion integrados con Telegram y Slack + Gmail


# 🚀 Sistema Automatizado de Gestión de Comunicados Compliance y Tax Automation

Este proyecto implementa un ecosistema de automatización para el procesamiento, validación y difusión multicanal de novedades impositivas y de compliance corporativo en Argentina, utilizando **n8n**, **Google Gemini** y **Notion**.

---

## 🔗 Enlaces Operativos
* **Dashboard de Control Operativo (Notion):** [(https://app.notion.com/p/3e51cdc143978005b8baf288fc5c2496?v=3e51cdc14397805cb216000c450df2c9&source=copy_link)]
* **Base RAG - Conocimiento Atómico (Notion):** [https://app.notion.com/p/3e51cdc14397803380bfd9ade51be1a1?v=3e51cdc1439780afad56000c47f2cab4&source=copy_link]

---

## 🛠️ Arquitectura del Flujo (n8n)
1. **Trigger de Entrada:** Captura actualizaciones en la base de datos de control de Notion.
2. **Filtro HITL (Human-in-the-Loop):** Validación estricta mediante la casilla `Aprobado = true` previa a la invocación del modelo de IA.
3. **Agente de IA (Google Gemini):** Generación de síntesis ejecutivas estructuradas en HTML compatible, respetando una restricción dura de 1.700 caracteres max.
4. **Distribución Multicanal:** Publicación simultánea en canales oficiales de **Telegram** y **Slack**.
5. **Manejo de Errores y Resiliencia:** 5 reintentos automáticos ante caídas de la API, registro de logs de error en Notion y alertas de correo crítico a soporte vía **Gmail**.

---

## 📁 Archivos en este Repositorio
* `workflow.json`: Exportación completa del flujo técnico en n8n.
* `Entrega Final Gomez Matías Com87415.pdf`: Documento de presentación técnica con diagrama, matriz de costos y manual operativo.
* `/evidencias/`: Capturas de pantalla demostrativas del flujo feliz, filtro HITL y ruta de errores.
* VIDEO EXPLICATIVO ---> [https://drive.google.com/file/d/13Bq8KjZcHSSnACJpAPQyXlq90Vbs3Suj/view?usp=sharing](url)

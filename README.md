# 📌 Levadur(IA)

**Un proyecto de código abierto desarrollado en n8n que integra inteligencia artificial y automatización para optimizar los procesos de reclutamiento, incluyendo la citación a exámenes médicos y la gestión de documentos.**

---

## 🧠 ¿Qué es Levadur(IA)?

Levadur(IA) es una solución automatizada para procesos de selección de personal, desarrollada sobre la plataforma de automatización n8n y ejecutada en un entorno local utilizando Docker. El sistema integra:

- Inteligencia artificial (Google Gemini) para interpretación de comandos en lenguaje natural.
- WhatsApp Business API para enviar mensajes automáticos a candidatos.
- Google Sheets como fuente de datos dinámica.

Este proyecto fue desarrollado como parte de una práctica organizacional universitaria para demostrar cómo la IA puede aplicarse de forma ética, eficiente y económica en contextos reales de Recursos Humanos.

---

## 🎯 Funcionalidades

- ✉️ **Notificación de exámenes médicos** personalizada vía WhatsApp.
- 📄 **Solicitud de documentos para contratación**.
- 🤖 **Asistente conversacional** con personalidad local (rolo/cachaco) para interpretar comandos como:
  - `"envía exámenes médicos"` → activa flujo `Examenes`
  - `"documentos para contratación"` → activa flujo `Documentos`
- 📊 **Integración con Google Sheets** como backend de datos de candidatos.
- 💵 **Optimización de costos** al ejecutarse localmente y usar Gemini por su bajo precio por token.

---

## ⚙️ Requisitos

- Docker (v20+)
- Cuenta de WhatsApp Business Cloud API
- Cuenta de Google Cloud con acceso a Sheets API
- Clave API de Google Gemini
- n8n (contenedorizado)

---

## 🚀 Instalación

```bash
git clone https://github.com/tuusuario/levadur-ia.git
cd levadur-ia
docker-compose up -d

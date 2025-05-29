# 📘 Manual de Usuario – Levadur(IA)

## 🧠 ¿Qué es Levadur(IA)?

Levadur(IA) es un sistema automatizado diseñado para apoyar procesos de selección de personal. Integra inteligencia artificial, mensajería vía WhatsApp y hojas de cálculo para agilizar la gestión de exámenes médicos y documentación de contratación.

Funciona como un asistente virtual que interpreta instrucciones del usuario y ejecuta flujos preconfigurados en **n8n**, alojados en un entorno local mediante **Docker**.

---

## 🖥️ Requisitos para el uso

- Sistema operativo: Windows, Linux o macOS
- Docker instalado (versión 20+)
- Conexión a internet para APIs externas
- Credenciales de:
  - Google Sheets API
  - WhatsApp Business API
  - Google Gemini API

---

## ⚙️ Instalación y configuración

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/tuusuario/levadur-ia.git
   cd levadur-ia


---

## Configura variables de entorno
Copia `.env.example` como `.env` y agrega tus credenciales:
```bash
cp .env.example .env
```
Llena las variables con tus claves reales en el archivo `.env`:
```makefile
WHATSAPP_API_KEY=
GOOGLE_SHEETS_CREDENTIALS=
GEMINI_API_KEY=
```
## Levanta el sistema
```bash
docker-compose up -d
```
## Accede a n8n
Abre tu navegador en [http://localhost:5678](http://localhost:5678) para ingresar a la interfaz de n8n.

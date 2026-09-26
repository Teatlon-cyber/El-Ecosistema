# Integration Telegram Bot

Escenario de [Make.com](https://www.make.com) para un bot de Telegram que identifica organismos (plantas, insectos, hongos, etc.) a partir de una foto enviada por el usuario, usando un modelo de IA para generar la respuesta.

## 🔧 Cómo funciona

1. El bot escucha nuevos mensajes en Telegram (`telegram:WatchUpdates`).
2. Un router evalúa si el mensaje trae una foto:
   - Si **no** trae foto → responde pidiendo que envíen una imagen del organismo.
   - Si **sí** trae foto → la envía a un modelo de IA para identificar el organismo y responde al usuario con el resultado.

## 🎥 Video demo

[![Ver video demo](https://img.youtube.com/vi/XT9WM7x41N0/0.jpg)](https://youtube.com/shorts/XT9WM7x41N0?feature=share)

▶️ [Ver en YouTube](https://youtube.com/shorts/XT9WM7x41N0?feature=share)

## 📁 Archivos

- [`Integration_Telegram_Bot_blueprint.json`](./Integration_Telegram_Bot_blueprint.json) — Blueprint exportado de Make.com. Puedes importarlo directamente en tu propia cuenta de Make: **Scenarios → Create a new scenario → Import Blueprint**.

## 📌 Notas

- Los identificadores `__IMTCONN__` y `__IMTHOOK__` dentro del blueprint son referencias internas de Make.com (conexión y webhook) y no contienen credenciales; al importar el blueprint deberás reconectar tu propia cuenta de Telegram y tu propio webhook.

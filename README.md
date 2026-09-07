# 🛡️ BaseMask
**La calculadora que en realidad es una bóveda secreta.**

App web de un solo archivo que parece una calculadora normal, pero esconde una bóveda de notas cifrada con **AES-256-GCM** real en el navegador.

## ✨ Características
- 🧮 Camuflaje total: parece una calculadora funcional.
- 🔐 Cifrado real: AES-256-GCM + PBKDF2 (120.000 iteraciones).
- 🧬 Cadena: nota → AES → Base64 → sello de fecha fusionado.
- 🖤 Pantalla negra señuelo al abrir notas (código a la vista, contenido no).
- 🗑️ Anti-intrusos: mantén Eliminar 5 s + tu código para desencriptar.
- 🆘 Rescate: mantén « . » 10 s (vibración) → código de rescate o destrucción total.
- ☁️ Backup: exporta/importa tu bóveda en un archivo Base64 con barra de progreso.
- 📱 Móvil-first: háptica, pantalla completa y modo discreto progresivo.

## 🚀 Cómo usarla
1. Abre `index.html` en cualquier navegador (mejor por HTTPS).
2. Crea tu clave secreta (4-12 dígitos) en la "calculadora".
3. Teclea tu clave + `=` para entrar en la bóveda.
4. Crea notas: texto, imagen, voz o enlaces. Todo se cifra solo.

## ⚠️ Aviso
Cifrado real sin servidor: si olvidas tu clave Y tu código de rescate, **no hay forma de recuperar las notas**. Ni el propio autor puede. Esa es la gracia.

## 🛠️ Tecnologías
HTML + CSS + JS vanilla · Web Crypto API · MediaRecorder · Firebase

---
Hecho con ☕ y paranoia saludable por [@djsemax](https://github.com/djsemax)
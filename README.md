<div align="center">

# 🔐 PGOsecure — Generador de Contraseñas Seguras

**Genera contraseñas ultra seguras directamente en tu navegador. 100% local, 100% privado.**

[![Netlify Status](https://api.netlify.com/api/v1/badges/f4393e05-dc4f-41a8-9c7e-8ecd87f5292e/deploy-status)](https://app.netlify.com/projects/pgosecure/deploys)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)

🌐 **[Demo en vivo → pgosecure.netlify.app](https://pgosecure.netlify.app/)**

</div>

---

## ✨ ¿Por qué PGOsecure?

La mayoría de generadores de contraseñas envían tus datos a servidores externos. **PGOsecure es diferente**: todo se ejecuta en tu navegador usando la [Web Crypto API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API). Tus contraseñas **nunca salen de tu dispositivo**.

### 🔑 6 Modos de Generación

| Modo | Descripción | Uso ideal |
|------|-------------|-----------|
| **Aleatoria** | Caracteres personalizables (mayúsculas, minúsculas, dígitos, símbolos) | Contraseñas estándar |
| **Passphrase** | 3 wordlists (EFF, PGP, BIP39) + palabras propias + leet speak | Contraseñas memorables |
| **Patrón** | Define tu propio patrón con repetición | Control total |
| **Pronunciable** | Fácil de recordar, difícil de adivinar | Uso diario |
| **WiFi** | Genera contraseña WiFi + QR code | Compartir WiFi seguro |
| **PIN** | Números puros para PINs | Dispositivos, apps |

### 🛡️ Verificador de Brechas HIBP

- Compara contraseñas generadas contra **[Have I Been Pwned](https://haveibeenpwned.com/)** usando **k-anonymidad** (solo envía los 5 primeros caracteres del SHA-1)
- Verifica **cualquier contraseña** que escribas — se borra inmediatamente tras la comprobación
- **Nunca se guarda en localStorage** ni se envía a ningún servidor

### 📊 Análisis de Entropía

- Calcula bits de entropía en tiempo real
- Estima tiempo de crackeo vs contraseñas comunes
- Tags de seguridad: 🔴 Muy débil → 🟡 Aceptable → 🟢 Fuerte → 🔵 Ultra

---

## 🚀 Cómo Usar

1. **Abre** [pgosecure.netlify.app](https://pgosecure.netlify.app/) en tu navegador
2. **Selecciona** el modo de generación (Aleatoria, Passphrase, etc.)
3. **Configura** los parámetros (longitud, caracteres, wordlist...)
4. **Genera** tu contraseña con un clic
5. **Verifica** si ha sido filtrada con el verificador HIBP

> 💡 **No necesitas instalar nada.** No hay servidor, no hay base de datos, no hay tracking.

---

## 🔒 Privacidad y Seguridad

```
✅ 100% local — todo se ejecuta en tu navegador
✅ Web Crypto API — generación criptográficamente segura
✅ k-anonymidad — HIBP nunca recibe tu contraseña completa
✅ Sin cookies de rastreo — solo cookies técnicas necesarias
✅ Sin analytics — no usamos Google Analytics
✅ Sin registro — no hay cuentas de usuario
✅ Open source — puedes verificar el código
```

### ¿Cómo funciona la verificación de brechas?

1. Tu contraseña se hashea con **SHA-1** en tu navegador
2. Solo se envían los **5 primeros caracteres** del hash a la API de HIBP
3. La API devuelve todos los hashes que empiezan por esos 5 caracteres
4. Tu navegador busca coincidencia **localmente**
5. La contraseña **nunca sale de tu dispositivo**

---

## 🛠️ Tecnología

- **HTML5** — monoarchivo, sin dependencias
- **JavaScript vanilla** — sin frameworks, carga instantánea
- **Web Crypto API** — generación criptográficamente segura
- **QRCode.js** — generación de QR codes (via CDN)
- **Inter + JetBrains Mono** — tipografías optimizadas
- **Netlify** — hosting gratis con HTTPS automático

---

## 📁 Estructura del Proyecto

```
password-generator/
├── index.html                              # App principal
├── img/
│   └── logo-pgosecure.png                  # Logo optimizado (26 KB)
├── netlify.toml                            # Headers seguridad + caché
├── sitemap.xml                             # 7 URLs indexables
├── aviso-legal.html                        # Aviso Legal (LSSI)
├── politica-privacidad.html                # Política Privacidad (RGPD)
├── politica-cookies.html                   # Política Cookies (LSSI)
├── como-crear-contraseña-segura.html       # Guía SEO
├── que-es-passphrase.html                  # Guía SEO
└── verificar-contraseña-filtrada.html      # Guía SEO
```

---

## 🌍 Legal

- **Aviso Legal** conforme al Art. 10 de la LSSI 34/2002
- **Política de Privacidad** conforme al RGPD 2016/679 y LOPDGDD 3/2018
- **Política de Cookies** conforme al Art. 22 de la LSSI
- Identidad: **PGOsecure** / PGOsecure@gmail.com (seudónimo, sin datos personales)

---

## 🚀 Despliegue

### En tu propia máquina

```bash
# Clona el repositorio
git clone https://github.com/TU-USUARIO/password-generator.git

# Abre index.html en tu navegador
# (no necesita servidor — funciona directamente como archivo local)
```

### En Netlify (gratis)

1. Arrastra la carpeta `password-generator` a [app.netlify.com/drop](https://app.netlify.com/drop)
2. Tu web estará en `https://tu-sitio.netlify.app/`
3. Configura un dominio propio para quitar el badge de Netlify

---

## 📄 Licencia

MIT License — usa, modifica y distribuye libremente.

---

## 🤝 Contribuir

Las contribuciones son bienvenidas. Puedes:

- Abrir un [Issue](https://github.com/TU-USUARIO/password-generator/issues) para reportar bugs
- Proponer nuevas funcionalidades
- Enviar un Pull Request

---

## 📧 Contacto

- **Web:** [pgosecure.netlify.app](https://pgosecure.netlify.app/)
- **Email:** PGOsecure@gmail.com

---

<div align="center">

**Si te ha sido útil, danos una ⭐ en GitHub**

Hecho con ❤️ para la comunidad de ciberseguridad

</div>

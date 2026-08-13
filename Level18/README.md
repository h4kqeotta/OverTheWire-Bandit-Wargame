# 🐧 Bandit Level 18 → Level 19

## 🎯 Objetivo
> <img width="1109" height="316" alt="56" src="https://github.com/user-attachments/assets/b28b9249-0597-47b6-ac5e-de2251388b99" />


---

## 🔎 Enumeración

La contraseña del siguiente nivel está en el archivo readme del directorio personal.

🎯 Objetivo: acceder al archivo y obtener la contraseña, pero evitando el problema de que .bashrc cierre la sesión automáticamente al conectarse por SSH.

🧠 Concepto: archivos de configuración de Bash y comportamiento de las sesiones SSH.

El usuario bandit18 tiene un .bashrc modificado que ejecuta un comando al iniciar sesión y cierra la conexión.

¿Qué está pasando?

Cuando haces:

ssh bandit18@bandit.labs.overthewire.org -p 2220

SSH:

Autentica tu contraseña ✅
Inicia sesión como bandit18 ✅
Ejecuta el shell de inicio (.bashrc) ❌
El .bashrc hace exit y te desconecta

Por eso ves todo el mensaje de bienvenida pero no puedes quedarte dentro.

Solución: ejecutar un comando directamente

SSH permite ejecutar un comando sin abrir una sesión interactiva.

Usa:

ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme

Te pedirá la contraseña de bandit18.

Después de introducirla, en vez de abrir el shell ejecutará directamente:

cat readme

y te mostrará la contraseña del siguiente nivel (bandit19).

<img width="644" height="266" alt="57" src="https://github.com/user-attachments/assets/5c85dc90-5c3a-41eb-b722-e6e5f2da48e2" />


🚩 Flag

KpsOfPkcP7i1FlIExk2QEjyt6dw8dxZI

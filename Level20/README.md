# 🐧 Bandit Level 20 → Level 21

## 🎯 Objetivo
> <img width="1087" height="342" alt="60" src="https://github.com/user-attachments/assets/6191f7e6-08dc-408b-bbdd-fa58dd9498e4" />


---

## 🔎 Enumeración

En este nivel hay un binario SetUID que se conecta a localhost usando el puerto que indiquemos.

🎯 Objetivo: hacer que el binario reciba la contraseña del nivel anterior y, si es correcta, obtener la contraseña del siguiente nivel.

🧠 Concepto: SetUID, conexiones de red locales y comunicación entre procesos/servicios.

Analicemos el enunciado:

"It makes a connection to localhost on the port you specify..."

➡️ El binario actúa como cliente. Tú debes proporcionarle un puerto.

"It then reads a line of text..."

➡️ El programa espera que haya un servidor escuchando en ese puerto y que le envíe la contraseña de bandit20.

"If the password is correct, it will transmit the password for the next level."

➡️ Si el servidor le envía la contraseña correcta, el binario responderá con la contraseña de bandit21.

Paso 1. Obtén la contraseña de bandit20
cat /etc/bandit_pass/bandit20

Guárdala.

Paso 2. Abre un puerto con nc

Supongamos que usarás el puerto 12345:

echo "CONTRASEÑA_DE_BANDIT20" | nc -l -p 12345

Reemplaza CONTRASEÑA_DE_BANDIT20 por la contraseña real.

Este comando deja a nc escuchando en el puerto 12345 y, cuando alguien se conecte, le enviará esa contraseña.

Si tu versión de nc no acepta -p, prueba simplemente:

echo "CONTRASEÑA_DE_BANDIT20" | nc -l 12345
Paso 3. Abre una segunda terminal

Conéctate otra vez como bandit20.

Paso 4. Ejecuta el binario SUID

En la segunda terminal:

./suconnect 12345

(El nombre puede variar; primero haz ls para ver cómo se llama el binario.)

El binario se conectará a tu servidor nc, recibirá la contraseña y, si es correcta, te devolverá la contraseña de bandit21.

Cualquier puerto menor a 1024, un usuario normal no tiene permisos.
<img width="955" height="244" alt="61" src="https://github.com/user-attachments/assets/b3cc53a8-5be0-441a-b55d-a3e41abf3910" />

<img width="561" height="302" alt="62" src="https://github.com/user-attachments/assets/21b5babd-4bb8-4658-8e83-f493525f21c5" />

<img width="948" height="130" alt="63" src="https://github.com/user-attachments/assets/df9a908c-910c-4b4b-89d1-79085dc17b87" />



🚩 Flag

bW9kBv5WC3P4yoDyf12LSdGuNz5ka6hY

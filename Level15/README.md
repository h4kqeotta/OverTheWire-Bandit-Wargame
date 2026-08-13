# 🐧 Bandit Level 15 → Level 16

## 🎯 Objetivo
> <img width="1052" height="282" alt="43" src="https://github.com/user-attachments/assets/316c4174-6303-4d57-a352-10e66abe35c5" />


---

## 🔎 Enumeración

En este nivel, la contraseña del siguiente nivel se obtiene enviando la contraseña actual al puerto 30001 de localhost.

🎯 Objetivo: enviar la contraseña utilizando una conexión protegida con SSL/TLS.

🧠 Concepto: conexiones seguras mediante SSL/TLS y comunicación con servicios de red.

Primero nos conectamos con el comando: 

openssl s_client -connect localhost:30001

Verás mucha información sobre el certificado y, al final, algo como:

CONNECTED(00000003)
...
---

Cuando la conexión quede abierta, pega la contraseña de bandit15 y presiona Enter.

Si la contraseña es correcta, el servidor responderá con la contraseña de bandit16.

<img width="498" height="43" alt="44" src="https://github.com/user-attachments/assets/efda22d2-9022-40de-8f4c-d28f44c63c58" />

<img width="721" height="443" alt="45" src="https://github.com/user-attachments/assets/e979530a-f51f-42d2-801e-19067ef96fa6" />

<img width="706" height="460" alt="46" src="https://github.com/user-attachments/assets/7bfa40b4-ef42-4038-9170-a1c68f06b329" />



🚩 Flag

kS0Hf0u5HiXFwKMKFqXvPdOTNGGa0X8V

# 🐧 Bandit Level 25 → Level 26

## 🎯 Objetivo
> <img width="1110" height="385" alt="81" src="https://github.com/user-attachments/assets/5fbdda47-d9d8-457b-a89d-d9c2338f52d2" />


---

## 🔎 Enumeración

En este nivel, debemos conectarnos como bandit26, pero su shell no es /bin/bash.

🎯 Objetivo: descubrir qué shell utiliza, entender cómo funciona y encontrar una forma de escapar de ella para acceder al sistema.

🧠 Concepto: shells de Linux, restricciones de acceso y técnicas para escapar de una shell limitada.


<img width="676" height="424" alt="82" src="https://github.com/user-attachments/assets/3e199a79-578f-4786-9853-b040d71cb39a" />

<img width="632" height="167" alt="83" src="https://github.com/user-attachments/assets/f217d158-c2fe-4665-a75a-8c81f6998646" />

more es un paginador de texto.

Cuando el contenido ocupa más de una pantalla, puedes entrar en modo interactivo.

Y dentro de more puedes ejecutar comandos.

Cuando estés dentro de more, presiona:

v

Esto abre el editor vi.

Dentro de vi escribe:

:set shell=/bin/bash

Enter.

Después:

:shell

Ahora tendrás una shell bash.

Comprueba:

whoami

Debería decir:

bandit26


<img width="436" height="301" alt="84" src="https://github.com/user-attachments/assets/c082f51b-afa7-497b-8a7b-40b3f65b461d" />

<img width="364" height="248" alt="85" src="https://github.com/user-attachments/assets/3e1b0a7c-3977-46c8-89fc-50316f45aec2" />



🚩 Flag

jHdv2ELQhT22BkprMNDjybZDAkw1zeBJ

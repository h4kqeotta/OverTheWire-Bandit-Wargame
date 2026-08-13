# 🐧 Bandit Level 11 → Level 12

## 🎯 Objetivo
> <img width="1009" height="249" alt="25" src="https://github.com/user-attachments/assets/9e858342-8103-46f7-a4c4-d9d5ea3d5a61" />


---

## 🔎 Enumeración

La contraseña del siguiente nivel está en data.txt, pero las letras fueron rotadas 13 posiciones.

🎯 Objetivo: descifrar el contenido aplicando ROT13 para obtener la contraseña.

🧠 Concepto: conocer y utilizar cifrados simples de sustitución como ROT13

Cada letra fue desplazada 13 posiciones en el alfabeto.

Ejemplo:

a → n
b → o
c → p
...
n → a

Como son 13 posiciones, ROT13 se puede aplicar dos veces y vuelve al texto original.
tr reemplaza caracteres.

Esta parte:

'A-Za-z'

representa todas las letras:

A-Z mayúsculas
a-z minúsculas

Y:

'N-ZA-Mn-za-m'

indica el desplazamiento ROT13:

Mayúsculas:

A-M → N-Z
N-Z → A-M

Minúsculas:

a-m → n-z
n-z → a-m

<img width="541" height="206" alt="26" src="https://github.com/user-attachments/assets/b3d4641f-bc76-443b-b00a-fabe32d3f675" />


🚩 Flag

GROozWPO8QyN0mGrjUkID0WCYkZiQxrN

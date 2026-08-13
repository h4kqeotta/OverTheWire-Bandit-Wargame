# 🐧 Bandit Level 12 → Level 13

## 🎯 Objetivo
> <img width="1086" height="278" alt="27" src="https://github.com/user-attachments/assets/b55c1086-7cb9-437e-84b5-b0f392c7d453" />


---

## 🔎 Enumeración
La contraseña está en data.txt, pero el archivo es un hexdump de un archivo comprimido varias veces.

🎯 Objetivo: reconstruir el archivo y descomprimirlo repetidamente hasta encontrar la contraseña.

🧠 Concepto: trabajar con hexdump, compresión y descompresión, utilizando un directorio temporal para realizar el proceso de forma segura.

La idea general es:

data.txt (hexdump)
        ↓
reconstruir archivo original
        ↓
identificar compresión
        ↓
descomprimir
        ↓
repetir hasta obtener la contraseña

<img width="600" height="344" alt="28" src="https://github.com/user-attachments/assets/631b2356-30a6-4e20-8263-6a523aa64852" />
<img width="352" height="56" alt="29" src="https://github.com/user-attachments/assets/f4a86399-b9f2-4599-b1c3-faa00a7cab99" />
<img width="529" height="216" alt="30" src="https://github.com/user-attachments/assets/6dfa9fe4-3810-4ef2-9f9f-31e5806e456f" />
<img width="949" height="361" alt="31" src="https://github.com/user-attachments/assets/dd342d70-94ca-4ab8-b207-895bab96266b" />
<img width="954" height="345" alt="32" src="https://github.com/user-attachments/assets/9c5187ba-ed24-44fd-a1a7-84d1c1413b67" />
<img width="603" height="374" alt="33" src="https://github.com/user-attachments/assets/a10d4bcb-c0ba-4523-b6ae-1fd75baab9e8" />
<img width="942" height="422" alt="34" src="https://github.com/user-attachments/assets/a3617c77-08b9-4ec8-91dd-5c5dc0e91596" />
<img width="727" height="216" alt="35" src="https://github.com/user-attachments/assets/01fac488-59a1-4ae1-822a-57459f12757f" />

🚩 Flag

qQYQiHOBPR8zR61qxYqX45quvihF2uzk

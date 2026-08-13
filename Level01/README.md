# 🐧 Bandit Level 01 → Level 02

## 🎯 Objetivo
> <img width="1129" height="245" alt="5" src="https://github.com/user-attachments/assets/bcc904da-b346-465b-864b-14ea47c22424" />


---

## 🔎 Enumeración

En este nivel la contraseña se encuentra en un archivo denominado "-" por lo que procedemos a buscarlo con el comando find y enviamos cualquier linea de error al /dev/null
<img width="452" height="66" alt="6" src="https://github.com/user-attachments/assets/56129f6a-94a2-4aa1-a4f9-398cfd09da39" />

```bash
find / -name "-" 2>/dev/null
cat /home/bandit1/-
```

🚩 Flag

PK8fYLZg2hnHSz83plBL1iEPKdD3QToB

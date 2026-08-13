# 🐧 Bandit Level 21 → Level 22

## 🎯 Objetivo
> <img width="1054" height="298" alt="64" src="https://github.com/user-attachments/assets/d47fe32b-8002-477f-ba99-bcebd84429b4" />


---

## 🔎 Enumeración

En este nivel, un programa se ejecuta automáticamente de forma periódica mediante cron.

🎯 Objetivo: revisar la configuración en /etc/cron.d/ para descubrir qué programa se ejecuta y cómo obtener la contraseña del siguiente nivel.

🧠 Concepto: tareas programadas con cron y análisis de configuraciones del sistema.


cron es el programador de tareas de Linux. Ejecuta comandos automáticamente en intervalos de tiempo.

El enunciado te dice exactamente dónde mirar:

Look in /etc/cron.d/

Paso 1. Lista los archivos
ls -l /etc/cron.d/

Verás varios archivos, por ejemplo:

cronjob_bandit22
cronjob_bandit23
cronjob_bandit24
...
Paso 2. Lee el archivo correspondiente

Como estás en el nivel 21 → 22, el archivo interesante es:

cat /etc/cron.d/cronjob_bandit22

Verás algo parecido a:

* * * * * bandit22 /usr/bin/cronjob_bandit22.sh

Eso significa que cada minuto se ejecuta el script:

/usr/bin/cronjob_bandit22.sh
Paso 3. Lee el script
cat /usr/bin/cronjob_bandit22.sh

El script tendrá una lógica similar a:

#!/bin/bash
chmod ...
cat /etc/bandit_pass/bandit22 > /tmp/...

o algo equivalente.

La idea es descubrir dónde copia la contraseña.

Paso 4. Lee el archivo de salida

Una vez que identifiques la ruta (normalmente en /tmp), simplemente haz:

cat /tmp/<nombre_del_archivo>

y obtendrás la contraseña de bandit22.

<img width="593" height="282" alt="65" src="https://github.com/user-attachments/assets/71ecd18d-ed40-4a6c-86fe-c77ef4f70afa" />

<img width="600" height="135" alt="66" src="https://github.com/user-attachments/assets/1e4fad19-516b-4cf8-bc16-94527e5203a4" />



🚩 Flag

RYVux2rHEm9tiXHmLFzuR7Vhx6AZQMEz

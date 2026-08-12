# 🐧 OverTheWire — Bandit

![Linux](https://img.shields.io/badge/Linux-000000?style=for-the-badge\&logo=linux\&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-121011?style=for-the-badge\&logo=gnubash\&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-8A2BE2?style=for-the-badge\&logo=hackthebox\&logoColor=white)
![OverTheWire](https://img.shields.io/badge/OverTheWire-Bandit-red?style=for-the-badge)

## 📌 Sobre el proyecto

Este repositorio documenta mi progreso y aprendizaje durante la resolución de **Bandit**, un wargame de **OverTheWire** diseñado para enseñar y reforzar conocimientos fundamentales de Linux, terminal y ciberseguridad.

A través de diferentes niveles, el desafío plantea problemas que requieren utilizar comandos, herramientas y técnicas de Linux para encontrar información, analizar archivos, manipular datos y descubrir las credenciales necesarias para avanzar.

El objetivo de este proyecto no es únicamente completar los niveles, sino **comprender las técnicas utilizadas y desarrollar habilidades prácticas en entornos Linux**.

---

## 🎯 Objetivos

* 🐧 Mejorar el manejo de Linux desde la terminal.
* 💻 Fortalecer conocimientos de Bash y comandos Unix.
* 🔎 Desarrollar habilidades de enumeración y análisis.
* 🔐 Comprender diferentes mecanismos de autenticación.
* 📂 Aprender a trabajar con archivos, permisos y directorios.
* 🔤 Practicar procesamiento y manipulación de texto.
* 🌐 Comprender conceptos básicos relacionados con SSH y redes.
* 🧠 Mejorar la capacidad de resolución de problemas.
* 🛡️ Aplicar conocimientos útiles para ciberseguridad y pentesting.

---

## 🧰 Tecnologías y herramientas

Durante el desarrollo de los desafíos se utilizan diferentes herramientas y comandos disponibles en Linux.

### Sistema operativo

* Linux
* Kali Linux

### Terminal / Shell

* Bash
* SSH

### Comandos utilizados

```bash
ls
cd
cat
file
find
grep
sort
uniq
strings
cut
tr
base64
tar
gzip
bzip2
xxd
chmod
chown
ps
```

### Otras herramientas

* Git
* OpenSSH
* Vim / Nano
* Hexdump
* Utilidades de compresión y procesamiento de archivos

---

## 📚 Conceptos aprendidos

Durante los niveles de Bandit se trabajan diferentes conceptos fundamentales:

| Área            | Conceptos                                   |
| --------------- | ------------------------------------------- |
| 🐧 Linux        | Sistema de archivos, directorios y comandos |
| 🔐 Seguridad    | Contraseñas, autenticación y permisos       |
| 📂 Archivos     | Lectura, búsqueda, modificación y análisis  |
| 🔎 Enumeración  | Identificación de información relevante     |
| 🔤 Texto        | `grep`, `sort`, `uniq`, `cut`, `tr`, etc.   |
| 🔢 Codificación | Base64, hexadecimal y otros formatos        |
| 📦 Compresión   | `tar`, `gzip`, `bzip2`, etc.                |
| 🌐 Redes        | SSH, puertos y conexiones                   |
| ⚙️ Procesos     | Procesos y servicios del sistema            |
| 🧠 Scripting    | Automatización mediante Bash                |

---

## 📁 Estructura del repositorio

Cada nivel se encuentra organizado individualmente para facilitar la navegación y documentación.

```text
bandit/
│
├── level00/
│   └── README.md
│
├── level01/
│   └── README.md
│
├── level02/
│   └── README.md
│
├── level03/
│   └── README.md
│
├── ...
│
└── level33/
    └── README.md
```

Cada nivel contiene una explicación del problema, el proceso utilizado para resolverlo y los comandos relevantes.

---

## 🧪 Metodología

Para cada desafío sigo una metodología similar:

```text
┌──────────────────┐
│ Analizar el      │
│ objetivo         │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ Enumerar el      │
│ entorno          │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ Identificar      │
│ información      │
│ relevante        │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ Investigar       │
│ herramientas     │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ Resolver el      │
│ desafío          │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ Documentar       │
│ el aprendizaje   │
└──────────────────┘
```

La intención es evitar depender únicamente de copiar soluciones y, en cambio, entender **por qué funciona cada comando o técnica**.

---

## 🏆 Progreso

* [x] Level 00
* [x] Level 01
* [x] Level 02
* [x] Level 03
* [x] Level 04
* [x] Level 05
* [x] Level 06
* [x] Level 07
* [x] Level 08
* [x] Level 09
* [x] Level 10
* [x] Level 11
* [x] Level 12
* [x] Level 13
* [x] Level 14
* [x] Level 15
* [x] Level 16
* [x] Level 17
* [x] Level 18
* [x] Level 19
* [x] Level 20
* [x] Level 21
* [x] Level 22
* [x] Level 23
* [x] Level 24
* [x] Level 25
* [x] Level 26
* [x] Level 27
* [x] Level 28
* [x] Level 29
* [x] Level 30
* [x] Level 31
* [x] Level 32
* [x] Level 33

> **Nota:** Bandit actualmente finaliza en el Level 33. El Level 34 todavía no existe.

---

## 🔐 Spoilers

Este repositorio contiene **soluciones y walkthroughs de los niveles de Bandit**.

Si estás realizando el wargame por primera vez, recomiendo intentar resolver cada desafío por cuenta propia antes de consultar las soluciones.

<details>
<summary>⚠️ Recomendación</summary>

Utilizar walkthroughs como último recurso. El verdadero aprendizaje está en investigar, probar comandos y comprender por qué una solución funciona.

</details>

---

## 📈 Habilidades desarrolladas

Este proyecto me permitió reforzar especialmente:

```text
Linux
 ├── Terminal
 ├── Bash
 ├── File System
 ├── Permissions
 └── Processes

Networking
 ├── SSH
 ├── Ports
 └── Connections

Security
 ├── Enumeration
 ├── Authentication
 ├── Encoding
 └── Information Gathering

Problem Solving
 ├── Analysis
 ├── Research
 ├── Debugging
 └── Automation
```

---

## 🚀 Próximos objetivos

Después de completar Bandit, el objetivo es continuar desarrollando conocimientos prácticos mediante:

* 🔥 CTFs
* 🏴 Hack The Box
* 🟢 TryHackMe
* 🌐 Pentesting Web
* 🔎 Enumeración de sistemas y redes
* 🐧 Administración avanzada de Linux
* 🛡️ Análisis de vulnerabilidades
* 💻 Scripting y automatización
* 🔐 Pentesting

---

## 📖 Sobre OverTheWire

**OverTheWire** ofrece diferentes wargames orientados al aprendizaje de seguridad informática mediante desafíos prácticos.

**Bandit** está especialmente orientado a personas que quieren aprender los fundamentos necesarios para trabajar con Linux y la terminal.

🌐 https://overthewire.org/wargames/bandit/

---

## 👨‍💻 Autor

**Matías Aranda**

Cybersecurity / Pentesting

Este repositorio forma parte de mi proceso de aprendizaje y práctica en **Linux, ciberseguridad y penetration testing**.

---

⭐ Si este repositorio te resulta útil, considera darle una estrella.

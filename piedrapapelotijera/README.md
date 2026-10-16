# 🎮 Mini Juego "Piedra, Papel o Tijera" con Persistencia de Datos (struct + fstream)

## 🏫 E.E.S.T. N.º 1 "Eduardo Ader" — Vicente López
* **Materia:** Laboratorio de Programación (LPR) — 5° Año 3° División (Grupos A-B)
* **Almna:** Alma lazarte
* **Ciclo Lectivo:** 2° Cuatrimestre - 2026
* **Profesor:** Mansilla Muñoz York Elías

---

## 👥 Integrantes del Grupo
* **[Apellido y Nombre Alumno 1]** - GitHub: `@[Usuario_GitHub]`
* **[Apellido y Nombre Alumno 2]** - GitHub: `@[Usuario_GitHub]`

---

## 🎯 Objetivos de la Actividad
El propósito fundamental de esta actividad de contingencia y continuidad pedagógica es comprender de forma práctica la diferencia entre la **Memoria RAM** (volátil) y el **Almacenamiento Secundario / Disco** (no volátil).

Para ello, implementamos un software interactivo en C++ que:
1. **Modela datos con `struct`:** Agrupa variables heterogéneas (`idPartida`, `jugador`, `eleccionJugador`, `eleccionIA`, `resultado`) en una sola entidad conceptual.
2. **Escritura en Disco (`ofstream`):** Persiste los resultados de las partidas en modo de adición (`ios::app`) para evitar la pérdida o sobrescritura de datos históricos.
3. **Lectura desde Disco (`ifstream`):** Recupera secuencialmente el historial completo almacenado en formato de texto delimitado por comas (CSV) y lo despliega formateado en la terminal de comandos.

---

## 📁 Estructura del Repositorio Obligatoria
El espacio de trabajo mantiene estrictamente la organización jerárquica de archivos solicitada en la guía de evaluación:

```text
piedrapapelotijera/
├── .gitattributes          # Normalización de finales de línea
├── .gitignore              # Exclusiones de binarios (.exe, *.out, .vscode/)
├── LICENSE                 # Licencia MIT Escolar
├── README.md               # Portada del proyecto con integrantes (Este archivo)
├── docs/                   # Entregables y documentación técnica
│   ├── InformeEEST1_LPR2026_ACT07_G03_Informe_v1.0.0.pdf   # Informe APA v7
│   ├── CHANGELOG.md        # Historial de versiones del software
│   └── manuales/
│       ├── manual_programador_v1.0.0.md
│       └── manual_usuario_v1.0.0.md
├── src/                    # Código fuente compilable
│   ├── main.cpp            # Código principal del juego en C++
│   └── historial_partidas.txt # Archivo de persistencia de datos generado
└── capturas/               # Evidencias de ejecución obligatorias (.png)
    ├── jugada_consola.png  # Captura del menú y partida en consola
    └── archivo_disco.png   # Captura del archivo .txt con datos persistidos
```

---

## 💻 Comandos de PowerShell para VS Code (Windows 10/11)
Para realizar una compilación limpia utilizando el compilador `g++` bajo el estándar moderno de compatibilidad **C++11**, ejecute secuencialmente los siguientes comandos en su terminal:

```bash
# 1. Compilación limpia y enlazado del binario ejecutable
g++ -std=c++11 src/main.cpp -o src/piedrapapelotijera.exe

# 2. Ejecución directa del mini juego desde la consola
.\src\piedrapapelotijera.exe
```

---

## 📡 Sincronización Git Dual-Remote (Dual-Push)
Este proyecto cumple con la pauta de despliegue dual obligatoria, subiendo de forma simultánea el código fuente compilable y la documentación técnica tanto a **GitHub** como a **GitLab**.

```bash
# Verificación de servidores remotos configurados
git remote -v

# Secuencia de subida a ambos servidores simultáneamente
git push origin main
```

---


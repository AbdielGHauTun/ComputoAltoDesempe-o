
## Tarea #990 Investigar sobre herramientas opensource para computo de alto desempeño

# Universidad Del Caribe

### ASIGNATURA:
*Cómputo de Alto Desempeño*

---

*Realizado por:*

- *Abdiel Gabriel Hau Tun*  
- *Matrícula:* 200300588  

---

*PRESENTADO A:*  
*Docente:* Ismael Jiménez Sánchez  

---
# Tarea #990 Investigar sobre herramientas opensource para computo de alto desempeño. 
**Tema:** Herramientas Open Source para Cómputo de Alto Desempeño (HPC)  
---

## 1. MPI (Message Passing Interface)

- **Descripción:**  
  Estándar para comunicación entre procesos en sistemas distribuidos. Permite que múltiples procesos en diferentes nodos trabajen colaborativamente.

- **Implementación:**  
  Implementaciones populares incluyen OpenMPI y MPICH. Se usa comúnmente con C, C++ o Fortran.

- **Ejemplo de uso:**  
  El supercomputador **MareNostrum** en España utiliza MPI para ejecutar simulaciones meteorológicas complejas, dividiendo el modelo climático entre cientos de nodos.

---

## 2. OpenMP (Open Multi-Processing)

- **Descripción:**  
  API para programación paralela en sistemas de memoria compartida, como CPUs multinúcleo. Facilita la paralelización de tareas con directivas sencillas.

- **Implementación:**  
  Se utiliza con compiladores compatibles como GCC o Intel Compiler. Se insertan directivas `#pragma omp` en el código fuente.

- **Ejemplo de uso:**  
  En **bioinformática**, herramientas como **BLAST** aprovechan OpenMP para comparar secuencias genéticas más rápidamente.

---

## 3. SLURM (Simple Linux Utility for Resource Management)

- **Descripción:**  
  Sistema de planificación y gestión de trabajos en clusters. Controla el uso de CPUs, memoria, nodos y el tiempo de ejecución.

- **Implementación:**  
  Se configura en sistemas multiusuario y se utiliza mediante scripts con instrucciones `#SBATCH`.

- **Ejemplo de uso:**  
  El supercomputador **Summit** en Oak Ridge National Laboratory utiliza SLURM para administrar tareas de simulación médica, física y genómica.

---

## 4. Singularity (ahora Apptainer)

- **Descripción:**  
  Sistema de contenedores para entornos HPC. Facilita la ejecución reproducible y segura de software sin necesidad de root.

- **Implementación:**  
  Los usuarios crean contenedores `.sif` con sus aplicaciones y dependencias. Compatible con SLURM y entornos de HPC.

- **Ejemplo de uso:**  
  El **Broad Institute** utiliza Singularity para ejecutar pipelines de análisis de ADN en distintos clústeres con resultados consistentes.

---

## 5. GNU Parallel

- **Descripción:**  
  Herramienta de línea de comandos que permite ejecutar múltiples comandos en paralelo en una misma máquina.

- **Implementación:**  
  Se instala desde el sistema de paquetes (`apt`, `brew`) y se usa con la sintaxis `parallel`.

- **Ejemplo de uso:**  
  Utilizada por científicos para procesar grandes volúmenes de imágenes satelitales, paralelizando tareas de análisis.

---

## 6. HPL (High Performance Linpack)

- **Descripción:**  
  Benchmark para medir el rendimiento de supercomputadoras resolviendo ecuaciones lineales. Es la base del ranking Top500.

- **Implementación:**  
  Usa bibliotecas BLAS y MPI para distribuir el cálculo en varios nodos.

- **Ejemplo de uso:**  
  Supercomputadoras como **Fugaku** y **Frontier** ejecutan HPL para demostrar su rendimiento en el ranking mundial.

---

## 7. PETSc (Portable, Extensible Toolkit for Scientific Computation)

- **Descripción:**  
  Biblioteca de estructuras de datos y rutinas para resolver ecuaciones diferenciales parciales en sistemas paralelos.

- **Implementación:**  
  Escrito en C, con bindings para Python y Fortran. Se integra con MPI para escalar a miles de núcleos.

- **Ejemplo de uso:**  
  Utilizado por investigadores en dinámica de fluidos para simular turbulencias en flujos de aire y agua.

---

## 8. CUDA (Compute Unified Device Architecture) - Open Source Toolkit

- **Descripción:**  
  Aunque originalmente cerrado, muchas herramientas basadas en CUDA ahora tienen versiones open source (como cuBLAS, cuDNN). Permite programar GPUs para acelerar cálculos.

- **Implementación:**  
  Se usa con C/C++ y Python mediante librerías como PyCUDA o Numba.

- **Ejemplo de uso:**  
  Utilizado en entrenamiento de redes neuronales profundas en GPUs para acelerar tiempos de procesamiento en proyectos de inteligencia artificial.

---

## 9. LAMMPS (Large-scale Atomic/Molecular Massively Parallel Simulator)

- **Descripción:**  
  Simulador open source para dinámica molecular. Diseñado para ejecutarse eficientemente en entornos paralelos.

- **Implementación:**  
  Se implementa con MPI y OpenMP para escalar simulaciones atómicas en clústeres.

- **Ejemplo de uso:**  
  Utilizado en simulaciones de materiales en laboratorios de nanotecnología y química computacional.

---

## 10. RAY

- **Descripción:**  
  Framework de computación distribuida para Python, enfocado en aplicaciones de aprendizaje automático y ciencia de datos.

- **Implementación:**  
  Permite desplegar tareas distribuidas en múltiples nodos sin necesidad de escribir código MPI/OpenMP.

- **Ejemplo de uso:**  
  Empresas como **Ant Financial** y **OpenAI** lo usan para escalar experimentos de aprendizaje por refuerzo en entornos HPC.

---

## Conclusión Personal.

Las herramientas open source para HPC permiten abordar desafíos científicos y técnicos a gran escala. Cada una cumple funciones críticas: desde la distribución de tareas (MPI, OpenMP), la gestión de recursos (SLURM), la ejecución reproducible (Singularity), hasta simulaciones científicas (LAMMPS, PETSc) o el entrenamiento de modelos de IA (RAY, CUDA). Su uso está presente en supercomputadoras, laboratorios de investigación y empresas tecnológicas líderes.

---




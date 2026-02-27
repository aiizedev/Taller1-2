# 🐶 Sistema Experto con Incertidumbre — Identificación de Razas de Perros

Este repositorio contiene un cuaderno de **Jupyter Notebook** donde se implementa un **sistema experto basado en reglas** con **incertidumbre** (Certainty Factors / Factores de Certeza) para sugerir la **raza más probable** de un perro a partir de rasgos observables. Hace referencia al taller 1 y 2 de la materia Técnicas de IA, de la UNAL

> La idea central: en la vida real los rasgos se describen con duda (“creo que es mediano”, “parece de pelo largo”), por lo que el sistema recibe **hechos con grado de certeza** y genera un **ranking de razas**.

---

## ✨ Características
- ✅ **Base de conocimiento**: reglas tipo **SI (rasgos) ENTONCES (raza)** con peso `CF_regla`.
- ✅ **Motor de inferencia**: **Forward Chaining (encadenamiento hacia adelante)**.
- ✅ **Manejo de incertidumbre**:  
  - AND con incertidumbre: `min(...)`  
  - Propagación: `CF_antecedentes × CF_regla`  
  - Combinación de evidencias múltiples: función `combinar_cf` (estilo MYCIN).
- ✅ **Módulo de explicación**: logs por raza con la traza de reglas activadas y sus aportes.
- ✅ **Tests**: casos claros, ambiguos, con conflicto e información insuficiente.

---

## 📁 Estructura del proyecto
- `WhoLetTheDogsOut.ipynb` — Cuaderno principal con implementación y pruebas.
- `malumabby.jpg` — Imagen usada en documentación (opcional).
- `docs/` (opcional) — HTML/recursos de documentación si los agregas.

---

## 🚀 Cómo ejecutar
1. Clona el repositorio:
   ```bash
   git clone <URL_DEL_REPO>
   cd <NOMBRE_DEL_REPO>

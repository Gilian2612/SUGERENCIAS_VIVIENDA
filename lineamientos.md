# Proyecto PTIA — Recomendador de Barrios en Bogotá

**Grupo 01** · Nicolás Prieto · William Santiago Ruiz Medina
Escuela Colombiana de Ingeniería Julio Garavito — Departamento de Ingeniería de Sistemas

---

## 1. Propósito del curso (según *Lineamientos Proyecto.pdf*)

Formular y desarrollar una solución basada en IA que responda a una problemática relevante, integrando conocimientos metodológicos, técnicos y éticos. En equipos de dos, con una **prueba de concepto funcional** que demuestre viabilidad técnica.

## 2. Hitos y entregables

| Hito | Semana | Documento | Prototipo | Código | Video |
|---|---|---|---|---|---|
| **1. Exploración** ✅ | 5 | Contexto y relevancia (secciones 1–4) | De papel | — | ≤ 5 min |
| **2. Problema y avance solución** ⏳ | 10 | Justificar enfoque metodológico y técnico (secciones 5–6) | **De interfaz** | Fuentes del diseño y del código (avance) | ≤ 5 min |
| **3. Solución y evaluación** | 16 | Diseñar, implementar y validar (secciones 7–8) | Funcional (MVP) | Versión final | ≤ 10 min + demo |

### Tipos de prototipo

| Prototipo | Definición | Objetivo | Características |
|---|---|---|---|
| De papel | Boceto simple en papel o herramienta básica | Explorar ideas y validar comprensión del problema | Visualiza interfaz y flujo |
| **De interfaz** | Versión preliminar de la interfaz | **Validar la experiencia de usuario** | **Navegable**; **simula funciones no implementadas**; base para el funcional |
| Funcional | Versión inicial con funciones implementadas | Demostrar viabilidad técnica | Funcionalidades reales aunque limitadas; base hacia el MVP |

## 3. Secciones del documento

| # | Sección | Hito | Preguntas guía |
|---|---|---|---|
| 1 | Introducción | 1 ✅ | Tres problemas de interés; ¿por qué PTIA? |
| 2 | Trabajos relacionados | 1 ✅ | Dos trabajos por problema (resultados y tecnología) |
| 3 | Descripción del problema | 1 ✅ | Criterios de selección; problema elegido |
| 4 | Justificación | 1 ✅ | Gran problema; por qué es importante |
| 5 | **Alcance y objetivos** | **2** | a) Problema que efectivamente se resuelve · b) Por qué es una simplificación adecuada · c) Objetivo general cuantitativo y cualitativo |
| 6 | **Diseño metodológico** | **2** | a) Estrategia general + justificación · b) Dónde está la inteligencia (conocimiento + razonamiento) · c) Herramienta + justificación · d) Arquitectura (componentes y relaciones) · e) Componente principal (detalle) |
| 7 | Análisis de resultados | 3 | Dos mejores casos de prueba; caso más significativo con análisis |
| 8 | Conclusiones | 3 | Dos aciertos y dos errores; tres conclusiones; trabajo futuro |

## 4. Resumen del Hito 1 (base para el Hito 2)

- **Problema elegido:** quien se muda a Bogotá o dentro de ella no sabe definir parámetros para buscar barrio (transporte, seguridad, precio, colegios/universidades, cercanía al trabajo, garaje) y termina decidiendo por opiniones de terceros.
- **Técnica:** KNN (aprendizaje supervisado/basado en instancias). Cada barrio es un punto en el espacio de características y el perfil del usuario es la consulta.
- **Datos previstos:** DANE, Metrocuadrado, Finca Raíz.
- **Prototipo de papel:** formulario con 5 sliders (1–5) para transporte, seguridad, precio de arriendo, cercanía a universidades y zonas verdes, y un top 3 de barrios con % de similitud.
- **Casos de uso:** CU1 ingresar preferencias · CU2 ver barrios recomendados · CU3 ver detalle «include» · CU4 comparar barrios «extend».

## 5. Checklist Hito 2 (semana 10)

- [ ] **Documento**, secciones 5 (Alcance y objetivos) y 6 (Diseño metodológico)
- [ ] **Prototipo de interfaz**, navegable, con las pantallas de CU1–CU4 (las funciones no implementadas se simulan)
- [ ] **Avance de la solución**
  - [ ] Dataset inicial de barrios/UPZ de Bogotá (fuentes documentadas)
  - [ ] Preprocesamiento y normalización de variables
  - [ ] Primer motor KNN funcionando sobre el dataset
  - [ ] Diagramas de diseño (arquitectura, casos de uso actualizados)
- [ ] **Video** de 5 minutos o menos presentando el avance

## 6. Estructura del repositorio

```
RUIZ-PTIA/
├── lineamientos.md                    ← este archivo
├── Lineamientos Proyecto.pdf          ← lineamientos oficiales del curso
├── Plantilla_Proyectos_PTIA_ECI_LaTeX/← plantilla LaTeX del informe (XeLaTeX)
├── Plantilla_Proyectos_PTIA_ECI (1).docx
├── RUIZ_PRIETO.docx                   ← documento Word del Hito 1
├── H1_RUIZ_PRIETO.docx.pdf            ← PDF entregado del Hito 1
├── Hito1_PrietoRuiz.pptx              ← presentación del Hito 1
├── CASOS DE USO INICIAL.png           ← diagrama de casos de uso
└── UI1.jpg, UI2.jpg                   ← prototipo en papel
```

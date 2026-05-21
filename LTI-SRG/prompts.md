# Prompt: Generación de Historias de Usuario, Backlog y Tareas

Dado el LTI-SRG.md adjuntado se te pedira realizar una serie de pasos. Actúa como un Senior Product Manager con experiencia en metodologías ágiles y definición de historias de usuario, backlog y generación de tickets.

---

## 1. Generación de Historias de Usuario

Genera las Historias de Usuario mínimas necesarias para construir el MVP.

### Cada Historia de Usuario debe incluir

- **Título**
- **User Story** en formato: “Como [usuario], quiero [acción], para [beneficio]”
- **Descripción breve**
- **Criterios de aceptación** en formato BDD:
  - Dado que [contexto]
  - Cuando [acción]
  - Entonces [resultado esperado]
- **Notas adicionales**
- **Tareas técnicas sugeridas**
- **Qué NO debe cambiar** o quedar fuera del alcance de esta historia
- **Escenarios comunes a considerar**:
  - Errores esperados
  - Validaciones
  - Estados vacíos
  - Permisos
  - Casos límite
- **Dependencias** con otras Historias de Usuario, si aplica

### Reglas

- Cada HU debe cumplir con checklist INVEST.
- Cada HU debe ser suficientemente pequeña para que un agente de IA pueda implementarla en 5-15 minutos.
- No agregues funcionalidades que no estén definidas en el PRD.
- Si una funcionalidad parece útil pero no esencial, colócala en **Post-MVP / V2**.
- Sugiere un orden de implementación para el MVP y justifica brevemente.
- Incluye una sección final de **“Non-goals”** con lo que queda fuera de alcance del MVP.

---

## 2. Creación de backlog

Con base en las Historias de Usuario generadas, crea un Product Backlog priorizado para construir el MVP.

### Formato

Presenta el backlog en formato de tabla.

### El backlog debe incluir

- ID de backlog
- Épica o módulo
- Historia de Usuario relacionada
- Prioridad: Alta / Media / Baja
- Impacto usuario/negocio: Alto / Medio / Bajo
- Urgencia: Alta / Media / Baja
- Tipo: Feature / Bug / Tech task / Research / UX
- Dependencias
- Estimación relativa: XS / S / M / L
- Orden sugerido de implementación
- Criterios de aceptación resumidos
- Definition of Ready
- Definition of Done
- Notas para desarrollo asistido por IA

### Reglas

- No agregues funcionalidades nuevas que no existan en el PRD o en las HU.
- Mantén separado lo que pertenece al MVP de lo que pertenece a Post-MVP / V2.
- Si una historia o backlog item es demasiado grande para implementarse en una sola sesión, divídela en tareas más pequeñas.
- Ordena el backlog por prioridad de implementación considerando:
  1. Necesidad para completar el flujo principal del MVP
  2. Impacto en usuarios finales y valor para negocio/producto
  3. Impacto en retención, atracción de usuarios, ingresos o diferenciación
  4. Urgencia
  5. Dependencias técnicas
- Si una historia aporta valor al negocio/producto pero no es necesaria para completar el flujo principal del MVP, no debe ir antes de las historias esenciales del usuario, salvo que sea una dependencia técnica, un requisito crítico o un riesgo que deba validarse temprano.
- Marca explícitamente qué elementos son bloqueantes para otros.
- Incluye una sección final con riesgos de implementación y recomendaciones de secuencia.

---

## 3. Creación de tareas/tickets

Con base en el Product Backlog priorizado, genera un plan de implementación para agentes de IA.

### Objetivo

Convertir el backlog en tareas pequeñas, secuenciales, verificables y seguras de implementar.

### Cada tarea debe incluir

- ID de tarea
- Backlog item relacionado
- Objetivo específico
- Contexto funcional breve
- Dependencias previas
- Archivos o módulos probables a revisar o modificar
- Instrucciones concretas para el agente
- Criterios de aceptación verificables
- Pruebas manuales sugeridas
- Resultado esperado al finalizar
- Qué NO debe modificar
- Riesgos o consideraciones técnicas

### Reglas

- Cada tarea debe poder completarse en 5-15 minutos.
- No agrupes múltiples funcionalidades en una sola tarea.
- No propongas refactors grandes salvo que sean indispensables.
- Mantén una secuencia incremental donde el sistema quede funcional después de cada tarea.
- Si existe un proyecto o código base, primero inspecciona la estructura antes de proponer archivos o cambios.
- No inventes rutas, archivos, componentes, endpoints o modelos si no existen o no han sido definidos previamente.
- Si una tarea depende de otra, indícalo explícitamente.
- Si una tarea requiere una decisión no definida en el PRD, HU o backlog, márcala como pregunta abierta antes de asumirla.
- Prioriza cambios mínimos, claros y fáciles de revisar.
- Al finalizar cada tarea, el agente debe reportar:
  - Archivos modificados
  - Cambios realizados
  - Cómo probarlo
  - Qué quedó fuera del alcance
  - Riesgos o pendientes detectados

### Formato sugerido por tarea

## Tarea [ID] — [Título]

**Backlog item relacionado:** [ID o nombre del backlog item]

**Objetivo:**  
[Describe exactamente qué debe lograrse.]

**Contexto funcional:**  
[Explica brevemente por qué existe esta tarea y qué parte del flujo del MVP habilita.]

**Dependencias previas:**  
[Lista tareas, historias o módulos que deben existir antes.]

**Archivos o módulos probables a revisar/modificar:**  
- [Archivo o módulo probable]
- [Archivo o módulo probable]

**Instrucciones para el agente:**  
1. Inspecciona la estructura actual del proyecto.
2. Identifica los archivos reales relacionados con esta tarea.
3. Implementa únicamente el cambio solicitado.
4. Mantén compatibilidad con lo ya implementado.
5. No modifiques funcionalidades fuera del alcance.

**Criterios de aceptación verificables:**  
- [Criterio verificable 1]
- [Criterio verificable 2]
- [Criterio verificable 3]

**Pruebas manuales sugeridas:**  
- [Paso de prueba 1]
- [Paso de prueba 2]
- [Resultado esperado]

**Qué NO debe modificar:**  
- [Elemento fuera de alcance]
- [Archivo, módulo o funcionalidad que no debe tocar]
- [Restricción importante]

**Resultado esperado al finalizar:**  
[Describe el estado esperado del sistema después de completar la tarea.]

**Riesgos o pendientes:**  
[Lista riesgos técnicos, decisiones pendientes o consideraciones.]
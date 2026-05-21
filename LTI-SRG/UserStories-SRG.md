# Prompt: Generación de Historias de Usuario, Backlog y Tareas

Actúa como un Senior Product Manager con experiencia en metodologías ágiles y definición de historias de usuario, backlog y generación de tickets.

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

---

## Prompt de respuesta

# LTI ATS — Historias de Usuario, Product Backlog y Plan de Implementación para Agentes de IA

> Documento generado con base en el archivo `LTI-SRG.md`.
>
> **Rol asumido:** Senior Product Manager con experiencia en metodologías ágiles, definición de historias de usuario, backlog y generación de tickets.
>
> **Alcance base tomado del SRG:** MVP 1 — gestión de ofertas, registro de candidatos, pipeline básico y roles.
>
> **Post-MVP / V2:** evaluaciones, entrevistas, notificaciones, reportes e integraciones externas.

---

## Índice

1. [Historias de Usuario mínimas para el MVP](#1-historias-de-usuario-mínimas-para-el-mvp)
2. [Product Backlog priorizado](#2-product-backlog-priorizado)
3. [Plan de implementación para agentes de IA](#3-plan-de-implementación-para-agentes-de-ia)
4. [Checklist final para agentes](#checklist-final-para-agentes)

---

# 1. Historias de Usuario mínimas para el MVP

## Orden sugerido de implementación del MVP

1. Base de roles y acceso.
2. Gestión básica de ofertas.
3. Configuración de etapas por oferta.
4. Registro de candidatos.
5. Creación de aplicación de candidato a oferta.
6. Visualización de pipeline.
7. Cambio de etapa/estado del candidato.
8. Consulta de detalle de candidato/aplicación.
9. Comentarios internos mínimos.
10. Validaciones y estados vacíos del flujo principal.

**Justificación:** primero se necesita una base mínima de acceso y datos maestros; después se habilita el flujo central del ATS:

```text
Crear vacante → Registrar candidato → Asociarlo a una vacante → Verlo en pipeline → Moverlo de etapa
```

---

## HU-01 — Acceso básico según rol

**User Story:**  
Como usuario del sistema, quiero acceder con un rol definido, para ver únicamente las funciones que me corresponden.

**Descripción breve:**  
Permite diferenciar acceso básico entre reclutador, hiring manager, evaluador y coordinador, usando los roles definidos en el SRG.

**Criterios de aceptación BDD:**

- **Dado que** un usuario tiene rol `reclutador`, **cuando** inicia sesión, **entonces** puede acceder a gestión de ofertas y candidatos.
- **Dado que** un usuario tiene rol `hiring_manager`, **cuando** accede al sistema, **entonces** puede consultar candidatos y pipeline.
- **Dado que** un usuario no tiene rol válido, **cuando** intenta acceder, **entonces** el sistema debe restringir el acceso.
- **Dado que** un usuario está inactivo, **cuando** intenta operar en el sistema, **entonces** no debe poder realizar acciones.

**Notas adicionales:**  
No se define un flujo avanzado de autenticación en el SRG; esta HU cubre control básico por rol.

**Tareas técnicas sugeridas:**

- Definir verificación de rol activo.
- Restringir acciones por tipo de usuario.
- Agregar mensajes de acceso denegado.
- Preparar permisos mínimos por módulo.

**Qué NO debe cambiar / fuera de alcance:**

- No implementar 2FA.
- No implementar recuperación de contraseña.
- No crear gestión avanzada de usuarios.
- No agregar nuevos roles fuera de los definidos.

**Escenarios comunes:**

- **Errores esperados:** usuario sin rol.
- **Validación:** rol debe pertenecer al enum definido.
- **Estado vacío:** sin usuarios activos.
- **Permisos:** solo roles válidos pueden operar.
- **Caso límite:** usuario activo pero empresa inactiva, queda como pregunta abierta si no está definido.

**Dependencias:**  
Ninguna.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-02 — Crear oferta de empleo en borrador

**User Story:**  
Como reclutador, quiero crear una oferta de empleo en borrador, para preparar una vacante antes de publicarla.

**Descripción breve:**  
Permite crear una oferta con información básica: título, descripción, ubicación, tipo de contrato y estado inicial.

**Criterios de aceptación BDD:**

- **Dado que** soy reclutador, **cuando** capturo los datos obligatorios de una oferta, **entonces** el sistema guarda la oferta en estado `borrador`.
- **Dado que** falta un campo obligatorio, **cuando** intento guardar, **entonces** el sistema muestra errores de validación.
- **Dado que** la oferta se guarda correctamente, **cuando** regreso al listado, **entonces** aparece como borrador.
- **Dado que** no soy reclutador, **cuando** intento crear una oferta, **entonces** el sistema bloquea la acción.

**Notas adicionales:**  
La publicación externa queda fuera del MVP mínimo.

**Tareas técnicas sugeridas:**

- Crear formulario básico de oferta.
- Validar campos obligatorios.
- Persistir oferta.
- Mostrar confirmación de guardado.

**Qué NO debe cambiar / fuera de alcance:**

- No publicar en job boards.
- No crear plantillas avanzadas.
- No agregar analítica de oferta.
- No crear workflow complejo de aprobación.

**Escenarios comunes:**

- **Errores esperados:** campos vacíos, tipo de contrato inválido.
- **Validaciones:** título, descripción, ubicación y tipo de contrato.
- **Estado vacío:** primera oferta creada.
- **Permisos:** solo reclutador o coordinador si se decide permitirlo.
- **Caso límite:** fecha de cierre anterior a fecha de publicación, si se captura.

**Dependencias:**  
HU-01.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-03 — Listar ofertas de empleo

**User Story:**  
Como reclutador, quiero ver un listado de ofertas, para dar seguimiento a las vacantes creadas.

**Descripción breve:**  
Muestra ofertas con información mínima: título, estado, ubicación, tipo de contrato y fecha de creación/publicación si existe.

**Criterios de aceptación BDD:**

- **Dado que** existen ofertas, **cuando** entro al módulo de ofertas, **entonces** veo una lista con sus datos principales.
- **Dado que** no existen ofertas, **cuando** entro al módulo, **entonces** veo un estado vacío claro.
- **Dado que** una oferta está cerrada, **cuando** aparece en el listado, **entonces** se identifica su estado.
- **Dado que** soy hiring manager, **cuando** accedo al listado, **entonces** puedo consultar ofertas permitidas sin editarlas.

**Notas adicionales:**  
El control fino de visibilidad por vacante puede dejarse mínimo para MVP.

**Tareas técnicas sugeridas:**

- Crear consulta/listado de ofertas.
- Agregar estado vacío.
- Mostrar etiquetas de estado.
- Restringir acciones según rol.

**Qué NO debe cambiar / fuera de alcance:**

- No agregar filtros avanzados.
- No agregar búsqueda compleja.
- No agregar paginación si el volumen inicial no lo requiere.
- No mostrar métricas avanzadas.

**Escenarios comunes:**

- **Errores esperados:** fallo al cargar ofertas.
- **Validaciones:** estados válidos.
- **Estado vacío:** sin ofertas.
- **Permisos:** edición solo para roles autorizados.
- **Caso límite:** muchas ofertas, queda para V2 si requiere paginación.

**Dependencias:**  
HU-01, HU-02.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-04 — Configurar etapas básicas de selección para una oferta

**User Story:**  
Como reclutador, quiero definir etapas básicas de selección para una oferta, para organizar el avance de candidatos.

**Descripción breve:**  
Permite agregar etapas simples asociadas a una oferta: nombre, orden y tiempo objetivo.

**Criterios de aceptación BDD:**

- **Dado que** existe una oferta, **cuando** agrego una etapa con nombre y orden, **entonces** queda asociada a esa oferta.
- **Dado que** intento guardar una etapa sin nombre, **cuando** confirmo, **entonces** el sistema muestra error.
- **Dado que** hay varias etapas, **cuando** consulto la oferta, **entonces** aparecen ordenadas.
- **Dado que** una etapa ya está en uso por candidatos, **cuando** intento eliminarla, **entonces** el sistema debe prevenir inconsistencias o pedir confirmación.

**Notas adicionales:**  
No se implementan workflows avanzados ni automatizaciones.

**Tareas técnicas sugeridas:**

- Crear alta básica de etapas.
- Asociar etapa a oferta.
- Validar orden y nombre.
- Mostrar etapas ordenadas.

**Qué NO debe cambiar / fuera de alcance:**

- No reglas complejas de workflow.
- No automatización de cambios de etapa.
- No plantillas de etapas.
- No evaluaciones técnicas.

**Escenarios comunes:**

- **Errores esperados:** etapa duplicada, nombre vacío.
- **Validaciones:** orden numérico, nombre requerido.
- **Estado vacío:** oferta sin etapas.
- **Permisos:** solo reclutador/coordinador.
- **Caso límite:** dos etapas con mismo orden.

**Dependencias:**  
HU-02.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-05 — Registrar candidato manualmente

**User Story:**  
Como reclutador, quiero registrar candidatos manualmente, para capturar perfiles recibidos fuera del sistema.

**Descripción breve:**  
Permite crear un candidato con nombre, correo, teléfono, origen, perfil y CV URL si aplica.

**Criterios de aceptación BDD:**

- **Dado que** soy reclutador, **cuando** ingreso los datos obligatorios del candidato, **entonces** el sistema crea el registro.
- **Dado que** falta nombre o correo, **cuando** intento guardar, **entonces** el sistema muestra error.
- **Dado que** el correo ya existe, **cuando** intento registrar al candidato, **entonces** el sistema debe advertir posible duplicado.
- **Dado que** el candidato se guarda, **cuando** consulto candidatos, **entonces** aparece en el listado.

**Notas adicionales:**  
Carga de CV como archivo puede quedar fuera si no hay infraestructura definida; se puede usar `cvUrl` como mínimo.

**Tareas técnicas sugeridas:**

- Crear formulario de candidato.
- Validar nombre y correo.
- Guardar candidato.
- Manejar posible duplicado por correo.

**Qué NO debe cambiar / fuera de alcance:**

- No carga avanzada de documentos.
- No parseo automático de CV.
- No integraciones externas.
- No enriquecimiento automático de perfil.

**Escenarios comunes:**

- **Errores esperados:** correo inválido, campos obligatorios.
- **Validaciones:** formato de correo.
- **Estado vacío:** sin candidatos.
- **Permisos:** solo reclutador/coordinador.
- **Caso límite:** candidato con varias aplicaciones.

**Dependencias:**  
HU-01.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-06 — Asociar candidato a una oferta

**User Story:**  
Como reclutador, quiero asociar un candidato a una oferta, para iniciar su proceso de selección.

**Descripción breve:**  
Crea una aplicación entre candidato y oferta, con estado inicial `nuevo` y etapa inicial.

**Criterios de aceptación BDD:**

- **Dado que** existe un candidato y una oferta, **cuando** asocio el candidato a la oferta, **entonces** se crea una aplicación.
- **Dado que** la oferta tiene etapas, **cuando** se crea la aplicación, **entonces** se asigna la primera etapa disponible.
- **Dado que** la oferta no tiene etapas, **cuando** intento asociar candidato, **entonces** el sistema debe indicar que falta configuración.
- **Dado que** el candidato ya está asociado a la misma oferta, **cuando** intento repetirlo, **entonces** el sistema evita duplicados.

**Notas adicionales:**  
Esta HU habilita el flujo principal del pipeline.

**Tareas técnicas sugeridas:**

- Crear relación aplicación candidato-oferta.
- Asignar estado inicial.
- Asignar etapa inicial.
- Validar duplicados.

**Qué NO debe cambiar / fuera de alcance:**

- No aplicar automáticamente desde formularios externos.
- No importar candidatos masivamente.
- No generar notificaciones automáticas.
- No calcular puntaje global avanzado.

**Escenarios comunes:**

- **Errores esperados:** candidato inexistente, oferta inexistente.
- **Validaciones:** no duplicar aplicación.
- **Estado vacío:** oferta sin candidatos.
- **Permisos:** reclutador/coordinador.
- **Caso límite:** candidato aplicado a múltiples ofertas.

**Dependencias:**  
HU-02, HU-04, HU-05.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-07 — Visualizar pipeline básico de candidatos por oferta

**User Story:**  
Como reclutador, quiero visualizar el pipeline de candidatos por oferta, para entender el estado del proceso de selección.

**Descripción breve:**  
Muestra candidatos agrupados por etapa o estado dentro de una oferta.

**Criterios de aceptación BDD:**

- **Dado que** una oferta tiene aplicaciones, **cuando** abro su pipeline, **entonces** veo los candidatos agrupados por etapa.
- **Dado que** una etapa no tiene candidatos, **cuando** veo el pipeline, **entonces** la etapa aparece vacía.
- **Dado que** no hay aplicaciones, **cuando** abro el pipeline, **entonces** veo un estado vacío.
- **Dado que** soy hiring manager, **cuando** consulto el pipeline, **entonces** puedo verlo sin modificarlo si no tengo permiso.

**Notas adicionales:**  
No requiere drag and drop para MVP; puede ser listado agrupado.

**Tareas técnicas sugeridas:**

- Consultar aplicaciones por oferta.
- Agrupar por etapa.
- Mostrar estado vacío.
- Respetar permisos por rol.

**Qué NO debe cambiar / fuera de alcance:**

- No drag and drop obligatorio.
- No métricas de conversión.
- No reportes.
- No filtros avanzados.

**Escenarios comunes:**

- **Errores esperados:** oferta inexistente.
- **Validaciones:** aplicación debe tener estado válido.
- **Estado vacío:** pipeline sin candidatos.
- **Permisos:** lectura para hiring manager, edición para reclutador.
- **Caso límite:** aplicación sin etapa asignada.

**Dependencias:**  
HU-06.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-08 — Cambiar etapa o estado de una aplicación

**User Story:**  
Como reclutador, quiero mover un candidato entre etapas, para reflejar el avance real del proceso.

**Descripción breve:**  
Permite actualizar etapa actual y estado de una aplicación.

**Criterios de aceptación BDD:**

- **Dado que** existe una aplicación, **cuando** cambio su etapa, **entonces** el sistema actualiza la etapa actual.
- **Dado que** el nuevo estado es válido, **cuando** guardo, **entonces** se actualiza la aplicación.
- **Dado que** intento mover a una etapa inexistente, **cuando** guardo, **entonces** el sistema muestra error.
- **Dado que** un usuario sin permiso intenta cambiar etapa, **cuando** ejecuta la acción, **entonces** el sistema la bloquea.

**Notas adicionales:**  
El motor de reglas debe ser simple; no automatizar decisiones.

**Tareas técnicas sugeridas:**

- Crear acción de cambio de etapa.
- Validar etapa pertenece a la oferta.
- Actualizar estado.
- Refrescar pipeline.

**Qué NO debe cambiar / fuera de alcance:**

- No automatizar movimientos.
- No enviar notificaciones automáticas.
- No crear evaluación.
- No generar score automático.

**Escenarios comunes:**

- **Errores esperados:** etapa inválida, aplicación inexistente.
- **Validaciones:** estado dentro del enum.
- **Estado vacío:** no aplica.
- **Permisos:** solo reclutador/coordinador.
- **Caso límite:** mover candidato rechazado.

**Dependencias:**  
HU-07.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-09 — Consultar detalle de candidato y aplicación

**User Story:**  
Como reclutador o hiring manager, quiero consultar el detalle de un candidato dentro de una oferta, para revisar su información antes de decidir avances.

**Descripción breve:**  
Muestra información del candidato, oferta, estado, etapa actual y datos básicos de la aplicación.

**Criterios de aceptación BDD:**

- **Dado que** existe una aplicación, **cuando** abro su detalle, **entonces** veo datos del candidato y su estado actual.
- **Dado que** el candidato tiene CV URL, **cuando** veo el detalle, **entonces** puedo visualizar la referencia.
- **Dado que** la aplicación no existe, **cuando** intento abrirla, **entonces** el sistema muestra error o no encontrado.
- **Dado que** soy usuario sin permiso, **cuando** intento acceder al detalle, **entonces** el sistema bloquea la consulta.

**Notas adicionales:**  
No incluye evaluación ni entrevistas para MVP 1.

**Tareas técnicas sugeridas:**

- Crear vista/consulta de detalle.
- Mostrar candidato + aplicación + oferta.
- Validar permisos.
- Manejar no encontrado.

**Qué NO debe cambiar / fuera de alcance:**

- No edición avanzada de perfil.
- No historial completo de cambios.
- No evaluaciones.
- No documentos adjuntos avanzados.

**Escenarios comunes:**

- **Errores esperados:** aplicación no encontrada.
- **Validaciones:** IDs válidos.
- **Estado vacío:** campos opcionales sin dato.
- **Permisos:** lectura por roles autorizados.
- **Caso límite:** candidato sin teléfono o CV URL.

**Dependencias:**  
HU-06.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## HU-10 — Agregar comentario interno básico a una aplicación

**User Story:**  
Como reclutador o hiring manager, quiero agregar comentarios internos a una aplicación, para colaborar con el equipo de selección.

**Descripción breve:**  
Permite registrar notas internas simples asociadas a una aplicación.

**Criterios de aceptación BDD:**

- **Dado que** existe una aplicación, **cuando** agrego un comentario, **entonces** queda registrado con autor y fecha.
- **Dado que** el comentario está vacío, **cuando** intento guardarlo, **entonces** el sistema muestra error.
- **Dado que** una aplicación tiene comentarios, **cuando** abro el detalle, **entonces** puedo verlos.
- **Dado que** un usuario sin permiso intenta comentar, **cuando** ejecuta la acción, **entonces** el sistema la bloquea.

**Notas adicionales:**  
Es una colaboración mínima; no incluye menciones ni notificaciones.

**Tareas técnicas sugeridas:**

- Crear registro de comentario interno.
- Asociarlo a aplicación.
- Mostrar lista de comentarios.
- Validar texto requerido.

**Qué NO debe cambiar / fuera de alcance:**

- No menciones.
- No edición/eliminación avanzada.
- No notificaciones.
- No archivos adjuntos.

**Escenarios comunes:**

- **Errores esperados:** comentario vacío.
- **Validaciones:** longitud mínima/máxima.
- **Estado vacío:** sin comentarios.
- **Permisos:** comentar solo roles autorizados.
- **Caso límite:** comentarios muy largos.

**Dependencias:**  
HU-09.

**Checklist INVEST:**  
Independiente, negociable, valiosa, estimable, pequeña y testeable.

---

## Post-MVP / V2

Estas funcionalidades existen en el SRG, pero no son esenciales para completar el flujo principal del MVP 1:

- Evaluaciones de entrevistas.
- Programación de entrevistas.
- Notificaciones automáticas.
- Reportes y analítica.
- Integraciones con job boards, LinkedIn o formularios externos.
- Comparativos avanzados de candidatos.
- Panel de métricas.
- Publicación externa automática.
- Almacenamiento avanzado y procesamiento de CVs.

---

## Non-goals del MVP

Queda fuera del MVP:

- Automatización avanzada del proceso de selección.
- Integraciones externas reales.
- Evaluaciones técnicas o formularios complejos.
- Reportes de conversión, origen y tiempos.
- Notificaciones automáticas.
- Gestión avanzada de usuarios, permisos granulares o auditoría.
- 2FA, SSO o autenticación empresarial.
- App móvil nativa.
- Drag and drop obligatorio en pipeline.
- Carga, parsing o análisis automático de CV.
- Employer branding.
- Onboarding posterior a contratación.

---

# 2. Product Backlog priorizado

## MVP

| ID Backlog | Épica / módulo | Historia relacionada | Prioridad | Impacto usuario/negocio | Urgencia | Tipo | Dependencias | Estimación | Orden | Criterios de aceptación resumidos | Definition of Ready | Definition of Done | Notas para desarrollo asistido por IA |
|---|---|---|---|---|---|---|---|---|---:|---|---|---|---|
| BL-01 | Roles y acceso | HU-01 | Alta | Alto | Alta | Tech task | Ninguna | S | 1 | Usuario con rol válido accede; usuario inválido/inactivo se bloquea | Roles definidos del SRG disponibles | Permisos básicos funcionando y probados | Bloqueante para todo el MVP |
| BL-02 | Ofertas | HU-02 | Alta | Alto | Alta | Feature | BL-01 | S | 2 | Reclutador crea oferta en borrador con validaciones | Campos obligatorios definidos | Oferta persistida y visible | No crear publicación externa |
| BL-03 | Ofertas | HU-03 | Alta | Alto | Alta | Feature | BL-02 | XS | 3 | Listado muestra ofertas y estado vacío | Existe modelo/estructura de oferta | Listado funcional con permisos | Mantener simple, sin filtros avanzados |
| BL-04 | Etapas | HU-04 | Alta | Alto | Alta | Feature | BL-02 | S | 4 | Oferta puede tener etapas ordenadas | Oferta creada previamente | Etapas creadas y listadas | Bloqueante para aplicaciones con etapa inicial |
| BL-05 | Candidatos | HU-05 | Alta | Alto | Alta | Feature | BL-01 | S | 5 | Reclutador registra candidato con validaciones | Campos de candidato definidos | Candidato creado y consultable | No implementar carga real de CV si no existe storage |
| BL-06 | Aplicaciones | HU-06 | Alta | Alto | Alta | Feature | BL-02, BL-04, BL-05 | S | 6 | Candidato se asocia a oferta sin duplicarse | Oferta, etapa y candidato existen | Aplicación creada con estado inicial | Bloqueante para pipeline |
| BL-07 | Pipeline | HU-07 | Alta | Alto | Alta | Feature | BL-06 | M | 7 | Pipeline muestra candidatos por etapa y estados vacíos | Aplicaciones existentes | Vista agrupada por etapa funcionando | No usar drag and drop como requisito |
| BL-08 | Pipeline | HU-08 | Alta | Alto | Alta | Feature | BL-07 | S | 8 | Reclutador cambia etapa/estado con validaciones | Pipeline visible | Cambio persistido y reflejado | No automatizar reglas avanzadas |
| BL-09 | Detalle aplicación | HU-09 | Media | Alto | Media | Feature | BL-06 | S | 9 | Usuario autorizado ve detalle de candidato/aplicación | Aplicación existente | Detalle consultable con manejo de errores | Útil para decisión, no bloquea creación inicial |
| BL-10 | Colaboración | HU-10 | Media | Medio | Media | Feature | BL-09 | S | 10 | Se agregan y consultan comentarios internos | Detalle de aplicación disponible | Comentarios guardados con autor/fecha | Sin menciones ni notificaciones |
| BL-11 | UX / validaciones | HU-02 a HU-10 | Alta | Medio | Alta | UX | BL-02 a BL-10 | S | 11 | Estados vacíos, errores y validaciones visibles | Flujo base implementado | Validaciones mínimas cubiertas | Puede implementarse incrementalmente por módulo |

---

## Post-MVP / V2

| ID Backlog | Épica / módulo | Historia relacionada | Prioridad | Impacto usuario/negocio | Urgencia | Tipo | Dependencias | Estimación | Orden | Criterios de aceptación resumidos | Definition of Ready | Definition of Done | Notas para desarrollo asistido por IA |
|---|---|---|---|---|---|---|---|---|---:|---|---|---|---|
| V2-01 | Entrevistas | Post-MVP | Media | Alto | Media | Feature | BL-06, BL-09 | M | 12 | Programar entrevista asociada a aplicación | Flujo de aplicación estable | Entrevista creada y visible | No iniciar antes del pipeline |
| V2-02 | Evaluaciones | Post-MVP | Media | Alto | Media | Feature | V2-01 | M | 13 | Registrar puntaje y comentario de evaluación | Entrevistas existentes | Evaluación guardada | Requiere definición de criterios |
| V2-03 | Notificaciones | Post-MVP | Media | Medio | Baja | Feature | BL-08, BL-10 | M | 14 | Notificar cambios relevantes | Eventos definidos | Notificaciones visibles | No bloquear MVP |
| V2-04 | Reportes | Post-MVP | Baja | Medio | Baja | Feature | BL-07, BL-08 | M | 15 | Métricas básicas de pipeline | Datos suficientes | Reporte simple generado | Depende de uso real |
| V2-05 | Integraciones externas | Post-MVP | Baja | Alto | Baja | Research / Feature | BL-02, BL-05, BL-06 | L | 16 | Recibir candidatos desde fuente externa | Fuente definida | Integración validada | Alto riesgo, validar después |

---

## Riesgos de implementación y recomendaciones de secuencia

### Riesgos principales

- Implementar funciones V2 antes del flujo base puede retrasar el MVP.
- No definir permisos mínimos desde el inicio puede generar retrabajo.
- Permitir candidatos sin relación clara con ofertas puede romper el pipeline.
- Crear etapas sin orden o sin validaciones puede provocar estados inconsistentes.
- Intentar implementar drag and drop, integraciones o reportes desde el inicio puede inflar el alcance.

### Recomendaciones

1. Construir primero el flujo lineal: oferta → etapas → candidato → aplicación → pipeline.
2. Mantener permisos simples, pero presentes desde el inicio.
3. No depender de integraciones externas para registrar candidatos.
4. Usar estados vacíos y validaciones mínimas en cada pantalla.
5. Postergar reportes, entrevistas, evaluaciones y notificaciones hasta estabilizar el flujo principal.

---

# 3. Plan de implementación para agentes de IA

> Como no se adjuntó un código base del proyecto, no se proponen rutas, archivos o endpoints reales.
>
> En cada tarea se indican **módulos probables** y se obliga al agente a inspeccionar primero la estructura antes de modificar algo.

---

## Tarea T-01 — Inspeccionar estructura del proyecto

**Backlog item relacionado:** BL-01

**Objetivo:**  
Identificar la estructura real del proyecto antes de implementar roles o módulos.

**Contexto funcional:**  
El MVP necesita permisos básicos por rol, pero no se deben inventar archivos, rutas ni endpoints.

**Dependencias previas:**  
Ninguna.

**Archivos o módulos probables a revisar/modificar:**

- Módulo de autenticación existente.
- Módulo de usuarios existente.
- Configuración de rutas o navegación.
- Capa de servicios/API si existe.

**Instrucciones para el agente:**

1. Inspecciona la estructura actual del proyecto.
2. Identifica framework, carpetas principales y patrones existentes.
3. Localiza dónde se gestiona usuario, sesión, rutas y permisos.
4. No implementes cambios todavía.
5. Reporta archivos candidatos para futuras tareas.

**Criterios de aceptación verificables:**

- Se lista la estructura principal del proyecto.
- Se identifican módulos reales relacionados con usuario/roles.
- Se reportan dudas o ausencias.
- No se modifica código.

**Pruebas manuales sugeridas:**

- Ejecutar el proyecto si hay instrucciones disponibles.
- Confirmar que no hay cambios en git.
- Revisar que el reporte incluya archivos reales.

**Qué NO debe modificar:**

- No crear archivos.
- No cambiar rutas.
- No cambiar lógica de autenticación.

**Resultado esperado al finalizar:**  
Existe un reporte técnico de estructura y puntos de modificación reales.

**Riesgos o pendientes:**  
Si no existe autenticación previa, debe marcarse como pregunta abierta.

---

## Tarea T-02 — Definir permisos mínimos por rol

**Backlog item relacionado:** BL-01

**Objetivo:**  
Crear o ajustar una definición mínima de permisos por rol usando los roles del SRG.

**Contexto funcional:**  
El MVP necesita restringir acciones entre reclutador, hiring manager, evaluador y coordinador.

**Dependencias previas:**  
T-01.

**Archivos o módulos probables a revisar/modificar:**

- Módulo real de permisos detectado.
- Configuración real de roles.
- Utilidades de autorización existentes.

**Instrucciones para el agente:**

1. Usa los archivos reales identificados en T-01.
2. Define permisos mínimos: crear oferta, ver oferta, crear candidato, ver pipeline, mover candidato, comentar.
3. No agregues roles nuevos.
4. Mantén la implementación simple.
5. Reporta cualquier permiso no definido en el PRD/SRG como pregunta abierta.

**Criterios de aceptación verificables:**

- Roles válidos están definidos.
- Permisos mínimos están centralizados o claramente ubicados.
- No se agregan roles ajenos al SRG.
- La implementación puede reutilizarse en tareas posteriores.

**Pruebas manuales sugeridas:**

- Validar usuario reclutador con permisos de edición.
- Validar hiring manager con permisos de consulta.
- Validar usuario sin rol válido.

**Qué NO debe modificar:**

- No implementar login nuevo.
- No agregar 2FA.
- No cambiar diseño visual.

**Resultado esperado al finalizar:**  
Permisos mínimos disponibles para proteger módulos del MVP.

**Riesgos o pendientes:**  
Puede requerir decisión si `coordinador` tiene permisos equivalentes a reclutador.

---

## Tarea T-03 — Crear estructura mínima de oferta

**Backlog item relacionado:** BL-02

**Objetivo:**  
Preparar el modelo, tipo o estructura mínima para representar una oferta.

**Contexto funcional:**  
La oferta es la base del flujo de reclutamiento.

**Dependencias previas:**  
T-01, T-02.

**Archivos o módulos probables a revisar/modificar:**

- Modelo o tipo de oferta existente.
- Servicio/API de ofertas si existe.
- Capa de datos o mock temporal si el proyecto usa mocks.

**Instrucciones para el agente:**

1. Identifica si ya existe entidad de oferta.
2. Agrega únicamente campos del SRG: título, descripción, ubicación, tipoContrato, estado, fechas si aplica.
3. Usa estado inicial `borrador`.
4. No agregues campos no definidos.
5. Mantén compatibilidad con patrones existentes.

**Criterios de aceptación verificables:**

- Oferta puede representarse con campos mínimos.
- Estado acepta `borrador`, `publicada`, `cerrada`.
- Tipo de contrato usa valores definidos.
- No se introducen campos innecesarios.

**Pruebas manuales sugeridas:**

- Crear objeto oferta válido.
- Intentar estado inválido.
- Intentar tipoContrato inválido si existe validación.

**Qué NO debe modificar:**

- No crear publicación externa.
- No agregar integraciones.
- No agregar reportes.

**Resultado esperado al finalizar:**  
El sistema cuenta con estructura mínima para ofertas.

**Riesgos o pendientes:**  
Si no hay backend o persistencia definida, usar patrón existente del proyecto y reportarlo.

---

## Tarea T-04 — Implementar creación básica de oferta en borrador

**Backlog item relacionado:** BL-02

**Objetivo:**  
Permitir que un reclutador cree una oferta en estado borrador.

**Contexto funcional:**  
Es el primer paso operativo del ATS.

**Dependencias previas:**  
T-03.

**Archivos o módulos probables a revisar/modificar:**

- Pantalla/formulario real de ofertas.
- Servicio real de ofertas.
- Validaciones existentes.

**Instrucciones para el agente:**

1. Identifica pantalla o módulo real donde crear ofertas.
2. Implementa captura mínima de datos.
3. Aplica validaciones obligatorias.
4. Guarda la oferta con estado `borrador`.
5. Restringe acción a rol autorizado.

**Criterios de aceptación verificables:**

- Reclutador puede guardar oferta válida.
- Oferta inválida muestra errores.
- Usuario no autorizado no puede crear.
- Oferta queda en estado `borrador`.

**Pruebas manuales sugeridas:**

- Crear oferta con todos los campos.
- Crear oferta sin título.
- Intentar crear con rol no autorizado.
- Confirmar que se ve en datos/listado si existe.

**Qué NO debe modificar:**

- No implementar publicación externa.
- No agregar filtros.
- No modificar módulos de candidatos.

**Resultado esperado al finalizar:**  
Se puede crear una oferta básica en borrador.

**Riesgos o pendientes:**  
Si no existe UI, marcar si se implementó en capa lógica o si falta pantalla.

---

## Tarea T-05 — Implementar listado básico de ofertas

**Backlog item relacionado:** BL-03

**Objetivo:**  
Mostrar ofertas creadas con estado y datos principales.

**Contexto funcional:**  
Permite al usuario continuar el flujo seleccionando una vacante.

**Dependencias previas:**  
T-04.

**Archivos o módulos probables a revisar/modificar:**

- Pantalla real de listado de ofertas.
- Servicio/consulta de ofertas.
- Componente de estado vacío.

**Instrucciones para el agente:**

1. Localiza el módulo real de ofertas.
2. Agrega listado simple con título, ubicación, tipoContrato y estado.
3. Agrega estado vacío si no hay ofertas.
4. Respeta permisos de lectura.
5. No agregues filtros avanzados.

**Criterios de aceptación verificables:**

- Se muestran ofertas existentes.
- Se muestra estado vacío.
- Los estados son visibles.
- Usuarios sin permiso no acceden.

**Pruebas manuales sugeridas:**

- Ver listado con ofertas.
- Ver listado sin ofertas.
- Ver con rol reclutador.
- Ver con rol hiring manager.

**Qué NO debe modificar:**

- No agregar búsqueda avanzada.
- No agregar paginación.
- No modificar creación de candidatos.

**Resultado esperado al finalizar:**  
El usuario puede consultar las ofertas existentes.

**Riesgos o pendientes:**  
Si el volumen de ofertas crece, la paginación queda para V2.

---

## Tarea T-06 — Crear estructura mínima de etapa

**Backlog item relacionado:** BL-04

**Objetivo:**  
Representar etapas de selección asociadas a una oferta.

**Contexto funcional:**  
Las etapas permiten ordenar el pipeline.

**Dependencias previas:**  
T-03.

**Archivos o módulos probables a revisar/modificar:**

- Modelo/tipo de etapa.
- Servicio de ofertas o etapas.
- Capa de datos relacionada con oferta.

**Instrucciones para el agente:**

1. Identifica si ya existe entidad o estructura de etapa.
2. Agrega campos mínimos: id, ofertaId, nombre, orden, tiempoObjetivo.
3. Asegura relación con oferta.
4. No agregues reglas complejas.
5. Reporta si no hay persistencia definida.

**Criterios de aceptación verificables:**

- Una etapa pertenece a una oferta.
- Una etapa tiene nombre y orden.
- El orden es numérico.
- No se crean etapas sin oferta.

**Pruebas manuales sugeridas:**

- Crear etapa válida.
- Intentar etapa sin nombre.
- Intentar etapa sin oferta.
- Validar ordenamiento.

**Qué NO debe modificar:**

- No crear automatizaciones.
- No crear entrevistas.
- No crear evaluaciones.

**Resultado esperado al finalizar:**  
Existe soporte mínimo para etapas de selección.

**Riesgos o pendientes:**  
Debe definirse si habrá etapas default o siempre manuales.

---

## Tarea T-07 — Agregar creación/listado de etapas por oferta

**Backlog item relacionado:** BL-04

**Objetivo:**  
Permitir crear y visualizar etapas asociadas a una oferta.

**Contexto funcional:**  
Sin etapas, una aplicación no puede tener etapa inicial.

**Dependencias previas:**  
T-06.

**Archivos o módulos probables a revisar/modificar:**

- Detalle real de oferta.
- Servicio real de etapas.
- Componente o sección de etapas.

**Instrucciones para el agente:**

1. Localiza dónde se muestra o edita una oferta.
2. Agrega sección mínima de etapas.
3. Permite agregar nombre y orden.
4. Lista las etapas ordenadas.
5. Valida duplicados o errores simples si el patrón existe.

**Criterios de aceptación verificables:**

- Se agregan etapas a una oferta.
- Se listan ordenadas.
- No se guarda etapa sin nombre.
- Solo usuario autorizado puede crear etapas.

**Pruebas manuales sugeridas:**

- Crear dos etapas.
- Confirmar orden.
- Intentar crear una etapa vacía.
- Probar usuario sin permiso.

**Qué NO debe modificar:**

- No implementar drag and drop.
- No automatizar estados.
- No modificar candidatos.

**Resultado esperado al finalizar:**  
Una oferta puede tener etapas básicas configuradas.

**Riesgos o pendientes:**  
Si se requiere edición/eliminación de etapas, debe separarse en otra tarea.

---

## Tarea T-08 — Crear estructura mínima de candidato

**Backlog item relacionado:** BL-05

**Objetivo:**  
Preparar modelo, tipo o estructura para candidatos.

**Contexto funcional:**  
El candidato es la entidad que se asociará a una oferta mediante una aplicación.

**Dependencias previas:**  
T-01.

**Archivos o módulos probables a revisar/modificar:**

- Modelo/tipo de candidato.
- Servicio de candidatos.
- Capa de datos o mocks.

**Instrucciones para el agente:**

1. Identifica si existe entidad de candidato.
2. Agrega campos mínimos del SRG: nombre, correo, teléfono, origen, perfil, cvUrl, fechaRegistro.
3. Valida correo como campo clave.
4. No agregues parsing ni carga de archivos.
5. Mantén cambios mínimos.

**Criterios de aceptación verificables:**

- Candidato tiene campos mínimos.
- Correo puede validarse.
- CV se representa como URL opcional.
- No se agregan campos fuera del SRG.

**Pruebas manuales sugeridas:**

- Crear candidato válido.
- Intentar correo inválido.
- Crear candidato sin CV URL.
- Validar estructura final.

**Qué NO debe modificar:**

- No crear integraciones.
- No implementar carga de CV.
- No modificar ofertas.

**Resultado esperado al finalizar:**  
Existe soporte mínimo para representar candidatos.

**Riesgos o pendientes:**  
Detección de duplicados puede ser simple por correo.

---

## Tarea T-09 — Implementar registro manual de candidato

**Backlog item relacionado:** BL-05

**Objetivo:**  
Permitir registrar un candidato manualmente.

**Contexto funcional:**  
El MVP no depende de formularios externos ni job boards.

**Dependencias previas:**  
T-08.

**Archivos o módulos probables a revisar/modificar:**

- Pantalla/formulario real de candidatos.
- Servicio real de candidatos.
- Validaciones.

**Instrucciones para el agente:**

1. Localiza módulo real de candidatos.
2. Agrega formulario mínimo.
3. Valida nombre y correo.
4. Guarda candidato.
5. Muestra error en caso de duplicado si existe mecanismo.

**Criterios de aceptación verificables:**

- Reclutador registra candidato válido.
- Nombre y correo son obligatorios.
- Correo inválido muestra error.
- Candidato queda disponible para asociarse a oferta.

**Pruebas manuales sugeridas:**

- Registrar candidato completo.
- Registrar candidato sin correo.
- Registrar candidato con correo inválido.
- Registrar candidato sin CV URL.

**Qué NO debe modificar:**

- No modificar pipeline.
- No crear aplicación automáticamente.
- No agregar carga de archivo.

**Resultado esperado al finalizar:**  
Se puede crear un candidato manualmente.

**Riesgos o pendientes:**  
Si se requiere deduplicación avanzada, queda fuera del MVP.

---

## Tarea T-10 — Crear estructura mínima de aplicación

**Backlog item relacionado:** BL-06

**Objetivo:**  
Representar la relación candidato-oferta como aplicación.

**Contexto funcional:**  
La aplicación conecta candidato con vacante y habilita pipeline.

**Dependencias previas:**  
T-03, T-06, T-08.

**Archivos o módulos probables a revisar/modificar:**

- Modelo/tipo de aplicación.
- Servicio de aplicaciones.
- Capa de datos relacionada.

**Instrucciones para el agente:**

1. Identifica si existe entidad aplicación.
2. Agrega campos mínimos: candidatoId, ofertaId, estado, puntajeGlobal, fechaAplicación, etapaActual.
3. Usa estado inicial `nuevo`.
4. Relaciona con candidato y oferta.
5. No agregues score automático.

**Criterios de aceptación verificables:**

- Aplicación relaciona candidato y oferta.
- Estado inicial puede ser `nuevo`.
- Etapa actual puede asignarse.
- No hay aplicación sin candidato u oferta.

**Pruebas manuales sugeridas:**

- Crear aplicación válida a nivel lógico.
- Intentar sin candidato.
- Intentar sin oferta.
- Validar estado inicial.

**Qué NO debe modificar:**

- No crear entrevistas.
- No crear evaluaciones.
- No generar reportes.

**Resultado esperado al finalizar:**  
Existe estructura mínima de aplicación.

**Riesgos o pendientes:**  
`puntajeGlobal` puede permanecer vacío o en cero para MVP.

---

## Tarea T-11 — Asociar candidato a oferta

**Backlog item relacionado:** BL-06

**Objetivo:**  
Crear una aplicación a partir de un candidato y una oferta.

**Contexto funcional:**  
Es el puente funcional entre registro de candidatos y pipeline.

**Dependencias previas:**  
T-07, T-09, T-10.

**Archivos o módulos probables a revisar/modificar:**

- Módulo real de candidatos.
- Módulo real de ofertas.
- Servicio real de aplicaciones.

**Instrucciones para el agente:**

1. Identifica flujo real para seleccionar candidato y oferta.
2. Implementa acción de asociar candidato a oferta.
3. Asigna primera etapa según orden.
4. Evita duplicados candidato-oferta.
5. Muestra error si la oferta no tiene etapas.

**Criterios de aceptación verificables:**

- Se crea aplicación válida.
- Se asigna estado `nuevo`.
- Se asigna primera etapa.
- No permite duplicado.
- No permite asociar si no hay etapas.

**Pruebas manuales sugeridas:**

- Asociar candidato a oferta con etapas.
- Intentar asociar dos veces.
- Intentar asociar a oferta sin etapas.
- Confirmar aplicación creada.

**Qué NO debe modificar:**

- No crear candidato automáticamente.
- No crear oferta automáticamente.
- No enviar notificaciones.

**Resultado esperado al finalizar:**  
Un candidato puede iniciar proceso en una oferta.

**Riesgos o pendientes:**  
Debe definirse desde qué pantalla se dispara la asociación si no existe UX.

---

## Tarea T-12 — Consultar aplicaciones por oferta

**Backlog item relacionado:** BL-07

**Objetivo:**  
Obtener las aplicaciones asociadas a una oferta.

**Contexto funcional:**  
Esta consulta alimenta el pipeline.

**Dependencias previas:**  
T-11.

**Archivos o módulos probables a revisar/modificar:**

- Servicio real de aplicaciones.
- Consulta por oferta.
- Módulo de pipeline si existe.

**Instrucciones para el agente:**

1. Localiza dónde consultar aplicaciones.
2. Implementa consulta filtrada por oferta.
3. Incluye datos mínimos de candidato y etapa.
4. Maneja oferta sin aplicaciones.
5. No agregues métricas.

**Criterios de aceptación verificables:**

- Se obtienen aplicaciones de una oferta.
- No se mezclan aplicaciones de otras ofertas.
- Se incluyen datos mínimos para mostrar pipeline.
- Si no hay aplicaciones, retorna lista vacía.

**Pruebas manuales sugeridas:**

- Consultar oferta con aplicaciones.
- Consultar oferta sin aplicaciones.
- Consultar oferta inexistente.
- Verificar que candidato/etapa estén disponibles.

**Qué NO debe modificar:**

- No cambiar estado de aplicaciones.
- No agregar reportes.
- No modificar creación de oferta.

**Resultado esperado al finalizar:**  
El sistema puede alimentar una vista de pipeline.

**Riesgos o pendientes:**  
Optimización de consultas queda fuera del MVP.

---

## Tarea T-13 — Mostrar pipeline agrupado por etapa

**Backlog item relacionado:** BL-07

**Objetivo:**  
Mostrar aplicaciones agrupadas por etapa dentro de una oferta.

**Contexto funcional:**  
Permite al reclutador visualizar el avance del proceso.

**Dependencias previas:**  
T-12.

**Archivos o módulos probables a revisar/modificar:**

- Vista real de pipeline.
- Detalle real de oferta.
- Componentes de lista/columna si existen.

**Instrucciones para el agente:**

1. Identifica lugar real para mostrar pipeline.
2. Agrupa aplicaciones por etapa.
3. Muestra cada candidato con información mínima.
4. Muestra etapas vacías.
5. Agrega estado vacío si no hay aplicaciones.

**Criterios de aceptación verificables:**

- Pipeline muestra etapas.
- Candidatos aparecen bajo su etapa.
- Etapas sin candidatos se ven vacías.
- Oferta sin candidatos muestra mensaje claro.

**Pruebas manuales sugeridas:**

- Ver pipeline con varios candidatos.
- Ver etapa sin candidatos.
- Ver oferta sin aplicaciones.
- Ver con rol hiring manager.

**Qué NO debe modificar:**

- No implementar drag and drop.
- No cambiar etapa aún.
- No agregar métricas.

**Resultado esperado al finalizar:**  
Pipeline básico visible y entendible.

**Riesgos o pendientes:**  
Diseño visual avanzado queda fuera del MVP.

---

## Tarea T-14 — Implementar cambio simple de etapa

**Backlog item relacionado:** BL-08

**Objetivo:**  
Permitir actualizar la etapa actual de una aplicación.

**Contexto funcional:**  
Refleja el avance real del candidato en el pipeline.

**Dependencias previas:**  
T-13.

**Archivos o módulos probables a revisar/modificar:**

- Servicio real de aplicaciones.
- Vista real de pipeline.
- Acción o control de cambio de etapa.

**Instrucciones para el agente:**

1. Localiza acción real de edición o actualización.
2. Permite seleccionar nueva etapa válida.
3. Valida que la etapa pertenezca a la misma oferta.
4. Persiste el cambio.
5. Refresca pipeline o estado local.

**Criterios de aceptación verificables:**

- Reclutador cambia etapa.
- Etapa inválida se rechaza.
- Pipeline refleja el cambio.
- Usuario sin permiso no puede cambiar etapa.

**Pruebas manuales sugeridas:**

- Mover candidato a segunda etapa.
- Intentar mover a etapa inexistente.
- Probar con usuario sin permiso.
- Recargar y confirmar persistencia.

**Qué NO debe modificar:**

- No enviar notificaciones.
- No calcular scores.
- No crear historial avanzado.

**Resultado esperado al finalizar:**  
Candidatos pueden avanzar de etapa manualmente.

**Riesgos o pendientes:**  
Debe definirse si se permite regresar a etapas anteriores.

---

## Tarea T-15 — Implementar cambio simple de estado

**Backlog item relacionado:** BL-08

**Objetivo:**  
Permitir actualizar estado de aplicación: nuevo, revisado, entrevista, oferta o rechazado.

**Contexto funcional:**  
El estado resume la situación del candidato en el proceso.

**Dependencias previas:**  
T-14.

**Archivos o módulos probables a revisar/modificar:**

- Servicio real de aplicaciones.
- Vista/detalle de aplicación.
- Validaciones de estado.

**Instrucciones para el agente:**

1. Usa los estados definidos en el SRG.
2. Permite actualizar estado manualmente.
3. Valida que el estado sea permitido.
4. Persiste el cambio.
5. No agregues automatizaciones.

**Criterios de aceptación verificables:**

- Estado válido se guarda.
- Estado inválido se rechaza.
- Cambio se refleja en pipeline/detalle.
- Permisos aplican correctamente.

**Pruebas manuales sugeridas:**

- Cambiar a `revisado`.
- Cambiar a `rechazado`.
- Intentar estado inválido.
- Confirmar persistencia tras recargar.

**Qué NO debe modificar:**

- No crear entrevistas automáticamente.
- No enviar emails.
- No generar notificaciones.

**Resultado esperado al finalizar:**  
La aplicación tiene estado actualizable manualmente.

**Riesgos o pendientes:**  
Puede haber duplicidad conceptual entre etapa y estado; mantener ambos simples.

---

## Tarea T-16 — Crear consulta de detalle de aplicación

**Backlog item relacionado:** BL-09

**Objetivo:**  
Obtener detalle combinado de aplicación, candidato y oferta.

**Contexto funcional:**  
Permite revisar información antes de decidir avances.

**Dependencias previas:**  
T-11.

**Archivos o módulos probables a revisar/modificar:**

- Servicio real de aplicaciones.
- Servicio real de candidatos.
- Servicio real de ofertas.

**Instrucciones para el agente:**

1. Identifica cómo se consultan entidades relacionadas.
2. Implementa consulta de aplicación por ID.
3. Incluye datos mínimos de candidato, oferta, estado y etapa.
4. Maneja aplicación no encontrada.
5. Aplica permisos de lectura.

**Criterios de aceptación verificables:**

- Se obtiene detalle válido.
- Incluye candidato, oferta y estado.
- Maneja no encontrado.
- Bloquea acceso no autorizado.

**Pruebas manuales sugeridas:**

- Consultar aplicación existente.
- Consultar ID inexistente.
- Consultar con usuario autorizado.
- Consultar con usuario no autorizado.

**Qué NO debe modificar:**

- No agregar comentarios aún.
- No agregar evaluaciones.
- No editar candidato.

**Resultado esperado al finalizar:**  
Existe base para mostrar detalle de aplicación.

**Riesgos o pendientes:**  
Si no hay routing definido, reportar pregunta abierta de navegación.

---

## Tarea T-17 — Mostrar detalle de aplicación

**Backlog item relacionado:** BL-09

**Objetivo:**  
Presentar en UI o capa equivalente el detalle de candidato/aplicación.

**Contexto funcional:**  
Ayuda al usuario a tomar decisiones dentro del pipeline.

**Dependencias previas:**  
T-16.

**Archivos o módulos probables a revisar/modificar:**

- Vista real de detalle.
- Componente real de candidato.
- Pipeline/listado desde donde se accede.

**Instrucciones para el agente:**

1. Identifica patrón real de navegación.
2. Muestra datos principales del candidato.
3. Muestra oferta, etapa y estado.
4. Muestra CV URL si existe.
5. Maneja campos opcionales vacíos.

**Criterios de aceptación verificables:**

- Se visualiza detalle de aplicación.
- Campos opcionales vacíos no rompen UI.
- CV URL se muestra si existe.
- No encontrado se maneja correctamente.

**Pruebas manuales sugeridas:**

- Abrir detalle desde pipeline.
- Ver candidato sin teléfono.
- Ver candidato sin CV URL.
- Abrir aplicación inexistente.

**Qué NO debe modificar:**

- No editar candidato.
- No crear evaluaciones.
- No agregar comentarios en esta tarea.

**Resultado esperado al finalizar:**  
Usuario autorizado puede consultar detalle.

**Riesgos o pendientes:**  
Diseño exacto depende del sistema existente.

---

## Tarea T-18 — Crear estructura de comentario interno

**Backlog item relacionado:** BL-10

**Objetivo:**  
Representar comentarios internos asociados a una aplicación.

**Contexto funcional:**  
Habilita colaboración mínima entre reclutador y hiring manager.

**Dependencias previas:**  
T-16.

**Archivos o módulos probables a revisar/modificar:**

- Modelo/tipo de comentario.
- Servicio de comentarios.
- Capa de datos.

**Instrucciones para el agente:**

1. Identifica si existe entidad de comentarios.
2. Agrega campos mínimos: aplicaciónId, autorId, texto, fechaCreacion.
3. Valida texto requerido.
4. Asocia comentario a aplicación.
5. No agregues menciones ni notificaciones.

**Criterios de aceptación verificables:**

- Comentario pertenece a aplicación.
- Comentario tiene autor y fecha.
- Texto vacío se rechaza.
- No hay comentario sin aplicación.

**Pruebas manuales sugeridas:**

- Crear comentario válido.
- Intentar comentario vacío.
- Crear comentario en aplicación inexistente.
- Validar autor.

**Qué NO debe modificar:**

- No crear notificaciones.
- No agregar menciones.
- No editar/eliminar comentarios.

**Resultado esperado al finalizar:**  
Existe soporte mínimo para comentarios internos.

**Riesgos o pendientes:**  
Edición y eliminación quedan fuera.

---

## Tarea T-19 — Agregar comentario desde detalle de aplicación

**Backlog item relacionado:** BL-10

**Objetivo:**  
Permitir capturar un comentario interno en el detalle de aplicación.

**Contexto funcional:**  
Completa la colaboración mínima del MVP.

**Dependencias previas:**  
T-17, T-18.

**Archivos o módulos probables a revisar/modificar:**

- Vista real de detalle de aplicación.
- Servicio real de comentarios.
- Componente de formulario simple.

**Instrucciones para el agente:**

1. Agrega formulario mínimo de comentario.
2. Valida texto no vacío.
3. Guarda comentario con autor actual.
4. Actualiza la lista tras guardar.
5. Respeta permisos.

**Criterios de aceptación verificables:**

- Usuario autorizado agrega comentario.
- Comentario vacío muestra error.
- Comentario aparece en detalle.
- Usuario sin permiso no puede comentar.

**Pruebas manuales sugeridas:**

- Agregar comentario válido.
- Intentar comentario vacío.
- Recargar detalle y confirmar persistencia.
- Probar con hiring manager si tiene permiso definido.

**Qué NO debe modificar:**

- No agregar menciones.
- No enviar notificación.
- No modificar pipeline.

**Resultado esperado al finalizar:**  
Se pueden registrar comentarios internos básicos.

**Riesgos o pendientes:**  
Longitud máxima de comentario debe definirse si no existe.

---

## Tarea T-20 — Revisar validaciones y estados vacíos del flujo MVP

**Backlog item relacionado:** BL-11

**Objetivo:**  
Asegurar que el flujo principal tenga validaciones y estados vacíos mínimos.

**Contexto funcional:**  
Evita que el MVP se sienta incompleto o se rompa en escenarios básicos.

**Dependencias previas:**  
T-04 a T-19.

**Archivos o módulos probables a revisar/modificar:**

- Módulo real de ofertas.
- Módulo real de candidatos.
- Módulo real de aplicaciones.
- Módulo real de pipeline.
- Componentes de error/estado vacío existentes.

**Instrucciones para el agente:**

1. Recorre el flujo oferta → etapas → candidato → aplicación → pipeline.
2. Identifica pantallas sin estado vacío.
3. Agrega mensajes mínimos sin rediseñar.
4. Revisa validaciones obligatorias.
5. No agregues nuevas funcionalidades.

**Criterios de aceptación verificables:**

- Oferta sin datos muestra estado vacío.
- Candidatos vacíos muestran estado vacío.
- Pipeline sin aplicaciones muestra estado vacío.
- Formularios muestran errores claros.
- Permisos denegados muestran mensaje o bloqueo.

**Pruebas manuales sugeridas:**

- Entrar sin ofertas.
- Crear oferta incompleta.
- Ver pipeline sin candidatos.
- Intentar acciones sin permiso.
- Asociar candidato a oferta sin etapas.

**Qué NO debe modificar:**

- No cambiar arquitectura.
- No agregar filtros.
- No agregar reportes.
- No implementar V2.

**Resultado esperado al finalizar:**  
El MVP queda navegable, validado y consistente para el flujo principal.

**Riesgos o pendientes:**  
Puede detectar deuda visual que debe anotarse, no resolverse si implica rediseño.

---

# Checklist final para agentes

Cada agente debe reportar al finalizar:

- Archivos modificados.
- Cambios realizados.
- Cómo probarlo.
- Qué quedó fuera del alcance.
- Riesgos o pendientes detectados.

---


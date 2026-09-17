# Problem / Solution Fit — SQUAD 1
## Sistema de préstamos de equipos tecnológicos

**Integrantes del squad:** CASTELLANOS FORERO JUAN ESTEBAN | PINEDA GONZALEZ JUAN ESTEBAN (SM) | RODRIGUEZ GUARNIZO JERFERSON DAVID | VERGARA PINILLOS JUAN PABLO | VARGAS CARVAJAL JULIAN CAMILO  (PO)
**Fecha:** [13/09/2026]
**Responsable de esta fase:** Julian Camilo Vargas Carvajal
---

## 1. Problema (formulación elegida)

### 1.1 Enunciado del problema

> La institución educativa carece de un canal formal único y de una fuente 
> única de verdad para la custodia de los equipos tecnológicos. Esto obliga 
> a usuarios y personal a improvisar "sistemas de sombra" (correos 
> informales, acuerdos verbales y hojas de cálculo locales paralelas) que 
> fragmentan la información, impiden la trazabilidad en tiempo real y 
> generan falsa escasez, fricción operativa y decisiones de compra sin 
> datos confiables.

### 1.2 Tipo de problema (Restricción 3 del caso)

- [x] Combinación: **Información + Proceso + Comunicación**

**Justificación por dimensión:**

| Dimensión | Por qué aplica | Evidencia |
|---|---|---|
| **Información (núcleo)** | No existe Single Source of Truth. El mismo equipo aparece con datos contradictorios en dos registros. | Restricción 1 del caso + `pestel.md` (factor Tecnológico) |
| **Proceso** | No hay protocolo formal de transferencia de custodia. El personal improvisa el registro. | `pain-points.md` (problema raíz #3) |
| **Comunicación** | La ausencia de canal único obliga a canales informales (correo, acuerdo verbal) y la asimetría de interés entre personal y usuarios agrava la desalineación. | Restricción 2 + `pain-points.md` (problema raíz #2) |
| **Inventario** | **NO es el núcleo.** El enunciado confirma que hay equipos; el problema es saber dónde están y en qué estado. | Enunciado del caso |

### 1.3 Evidencia que sostiene el problema

| Evidencia | Fuente | ¿Validada o supuesto? |
|---|---|---|
| Un mismo equipo aparece con información diferente en dos registros | Enunciado del caso (Restricción 1) | **Validada** |
| Convivencia de formularios, hojas de cálculo y correos como canales de registro | Enunciado + `pain-points.md` | **Validada** |
| Retrasos en devoluciones y correos sin responder | Enunciado + `pain-points.md` | **Validada** |
| El personal operativo tiene menor interés que los usuarios (asimetría) | Enunciado (Restricción 2) | **Validada** |
| Ausencia de normalización (3NF) y de Single Source of Truth | `pestel.md` (factor Tecnológico) | **Validada** (técnica) |
| La ineficiencia genera "falsa escasez" y compras innecesarias | `pestel.md` (factor Económico) | **Supuesto** — no cuantificado |
| Los usuarios y personal crean "sistemas de sombra" por falta de canal formal | Inferencia del equipo a partir de la Restricción 1 | **Supuesto** — requiere validación |

> **Recordatorio de la actividad:** la IA no puede ser citada como evidencia de que un problema existe. Solo cuentan el enunciado, entrevistas, observaciones o documentos.

---

## 2. Afectados (stakeholders impactados)

| Stakeholder | Tipo | Cómo le afecta el problema | Nivel de afectación |
|---|---|---|---|
| **Estudiantes** | Primario | Llegan al mostrador y no encuentran el equipo que el sistema marca como disponible. Pérdida de clases y entregas. | **Alto** |
| **Docentes** | Primario | Planifican actividades con equipos que no llegan a tiempo. | **Alto** |
| Personal de préstamos | Secundario | Doble registro manual, carga operativa, tensión con usuarios. | Alto |
| Coordinador TI / Dirección | Clave | Sin datos consolidados para auditar inventario ni decidir compras. | Medio |
| Área financiera / Compras | Secundario | Riesgo de compras duplicadas por falsa escasez. | Medio |
| Personal de mantenimiento | Secundario | No sabe qué equipos requieren revisión porque no hay estado actualizado. | Bajo |

**Stakeholder principal afectado:** **Estudiantes.**

**Justificación:** son los usuarios finales con mayor frecuencia de uso, menor poder de decisión y quienes sufren directamente la "falsa escasez" en el mostrador. La IA en la Formulación 1 cometió el error de justificar al estudiante como afectado por la violación de 3NF — eso es un dolor de TI, no del estudiante. El equipo corrigió el enfoque: **al estudiante le afecta no encontrar el equipo, no la normalización de la base de datos.**

---

## 3. Propuesta de valor

### 3.1 ¿Cómo el sistema cambia/mejora la situación actual?

> Un sistema que centralice en una **Single Source of Truth** el ciclo completo 
> de préstamo y devolución, con trazabilidad en tiempo real de la custodia, 
> alertas automáticas de vencimiento y reportes consolidados para la 
> dirección. Esto elimina la duplicidad de registros (Restricción 1), reduce 
> la fricción operativa del personal (Restricción 2) y da a la institución 
> datos confiables para decidir compras y mantenimiento.

### 3.2 ¿Qué necesidad urgente resuelve?

1. **Para el estudiante:** saber con certeza si un equipo está disponible **antes** de solicitarlo.
2. **Para el personal:** un solo canal de registro, sin doble digitación ni persecución de correos.
3. **Para la dirección:** datos agregados y auditables sobre uso real, retrasos y estado del inventario.

### 3.3 ¿Qué NO resuelve (límites)?

- No resuelve la falta de equipos si la demanda supera la oferta real.
- No reemplaza el mantenimiento físico ni la reposición de hardware.
- No garantiza adopción del personal si no se gestiona el cambio y se alinean incentivos (Restricción 2).
- No elimina por sí solo los "sistemas de sombra" si el canal formal no es más rápido que el informal.

---

## 4. Alternativas descartadas

### Alternativa A — Formulación 1 original (IA)
> "La ausencia de una Single Source of Truth y el uso desarticulado de 
> formularios, correos y hojas de cálculo provocan una asimetría crítica en 
> el estado de los equipos, violando la integridad de datos."

**Decisión:** **MODIFICADA** (se adoptó como base, pero se reformuló).

**Por qué no se aceptó tal cual:**
- Usa lenguaje técnico (3NF, Single Source of Truth) que no es comprensible para el stakeholder principal (estudiante).
- Ignora la Restricción 2 (asimetría de interés del personal).
- La evidencia que pide (auditoría de discrepancias) solo mide el tamaño del desastre, no la causa.
- **Aporte conservado:** la dimensión de información desfragmentada es el núcleo del problema.

### Alternativa B — Formulación 2 (IA)
> "La brecha entre la urgencia operativa de los usuarios solicitantes y la 
> baja motivación del personal de préstamos deteriora la ejecución de los 
> protocolos."

**Decisión:** **RECHAZADA.**

**Por qué:**
- La propia IA la identificó como la **más débil** de las tres.
- Reduce un problema sistémico de gestión de activos a un juicio sobre la actitud del personal (terreno de recursos humanos, no de análisis de sistemas).
- Asume que la baja motivación es causa, cuando podría ser **consecuencia** de la ineficiencia de las herramientas actuales.
- Ignora la Restricción 1 (contradicción de registros).
- Malidentifica al stakeholder: el personal no sufre el problema, su desinterés sugiere que el estado actual le genera menos fricción que adoptar un protocolo estricto.
- **Evidencia que propone (medir tiempos de correo) es métrica de desempeño individual, no evidencia sistémica.**

### Alternativa C — Formulación 3 (IA)
> "La carencia de un protocolo estandarizado para registrar la transferencia 
> de custodia impide conocer la ubicación real de los dispositivos."

**Decisión:** **RECHAZADA.**

**Por qué:**
- Es **tautológica**: "falta protocolo porque no hay control, y no hay control porque falta protocolo". No aporta causa raíz.
- Ignora la Restricción 1 (contradicción de registros).
- Malidentifica al stakeholder principal: dirige el impacto a Dirección/TI, cuando el dolor inmediato recae en el estudiante.
- **Aporte conservado:** la dimensión de proceso (falta de protocolo de custodia) se integró en la formulación final.

### Alternativa D — "Shadow Systems" (omitida por la IA, propuesta por el equipo)
> "La carencia de un canal formal, unificado e inmediato obliga a usuarios y 
> personal a improvisar sistemas de sombra (correos informales, acuerdos 
> verbales, hojas de cálculo locales paralelas), fragmentando la custodia y 
> perdiendo la propiedad legal de los activos."

**Decisión:** **ADOPTADA parcialmente** (integrada a la formulación final).

**Por qué:**
- Expone un ángulo que la IA no consideró: los formularios y Excel actuales **no son herramientas deficientes per se**, sino **parches informales** creados por la comunidad ante la ausencia de un canal oficial funcional.
- Conecta la Restricción 1 (registros contradictorios) con la Restricción 2 (desinterés del personal) sin caer en juicios de valor.
- **No se adoptó como formulación única** porque por sí sola no cubre la dimensión de información (Single Source of Truth).

### Alternativa final elegida
> **Síntesis:** Formulación 1 (información desfragmentada) + Shadow Systems 
> (improvisación por ausencia de canal formal) + dimensión de proceso 
> (falta de protocolo de custodia), redactada en lenguaje comprensible para 
> el stakeholder principal.

---

## 5. Tabla "IA propone → equipo verifica → evidencia → decisión"

| Elemento analizado | Propuesta IA | Qué verificamos | Decisión del equipo | Razón / evidencia |
|---|---|---|---|---|
| Formulación 1 (Fragmentación estructural) | Problema = violación de 3NF y ausencia de SSOT | Comprensibilidad para el stakeholder principal + cobertura de Restricción 2 | **Modificada** | Se conservó el núcleo de información, pero se reformuló sin jerga técnica e incorporando la dimensión de proceso |
| Formulación 2 (Desalineación operacional) | Problema = baja motivación del personal | Coherencia con Restricciones 1 y 2 + evidencia propuesta | **Rechazada** | La IA misma la señaló como la más débil. Desvía el problema hacia RR.HH. y no ofrece palanca de ingeniería |
| Formulación 3 (Protocolo de trazabilidad) | Problema = falta de protocolo | Coherencia lógica + stakeholder afectado | **Rechazada** | Es tautológica. Malidentifica al stakeholder principal. Su dimensión de proceso se integró a la formulación final |
| Shadow Systems (omitida por IA) | — | Conexión con Restricción 1 y 2 | **Adoptada parcialmente** | Aporta la causa de la fragmentación: ausencia de canal formal funcional |
| Stakeholder principal | IA puso estudiantes/docentes (F1), personal (F2), dirección (F3) | Poder/interés + experiencia directa del dolor | **Estudiantes** | Sufren la falsa escasez directamente. El personal no sufre el problema; la dirección solo impacto indirecto |
| Tipo de problema | IA propuso "información e inventario" (F1), "proceso y comunicación" (F2), "proceso e información" (F3) | Restricciones 1, 2 y 3 | **Información + Proceso + Comunicación** | La información es el núcleo; el proceso y la comunicación son dimensiones agravantes |
| Evidencia requerida | Auditoría de discrepancias (F1), tiempos de correo (F2), mapeo de flujo (F3) | Fuerza probatoria de cada evidencia | **Reformulada** | Se conserva la auditoría de registros, pero se añade observación directa y entrevistas |

> **Propuesta de IA rechazada (obligatoria):** la Formulación 2 completa. 
> Se rechazó porque reduce un problema sistémico de gestión de activos a un 
> diagnóstico actitudinal del personal, desviando el presupuesto hacia 
> capacitaciones o cambios de actitud en lugar de corregir la arquitectura 
> de la información y el proceso de custodia.

---

## 6. Reflexión sobre el uso de IA (Nivel 3)

### ¿En qué se equivocó o quedó corta la IA?

1. **Confundió el lenguaje técnico con el problema del negocio.** La IA habló de 3NF y Single Source of Truth, pero el stakeholder principal (estudiante) no sufre por la normalización; sufre porque no encuentra el equipo.
2. **Propuso una formulación basada en la actitud del personal** (Formulación 2), que la propia IA luego calificó como la más débil. Eso evidencia que la primera generación de alternativas fue inconsistente.
3. **Fue tautológica en la Formulación 3**: "falta protocolo" es una descripción del síntoma, no una causa raíz.
4. **Omitió el ángulo de los "sistemas de sombra"**, que resultó ser la pieza que conectaba las dos restricciones del caso.

### ¿Qué aportó el equipo que la IA no podía decidir por sí sola?

1. **La traducción del problema al lenguaje del stakeholder.** El equipo reformuló la Formulación 1 para hablar de "falsa escasez" y "sistemas de sombra", no de 3NF.
2. **La detección de la tautología** en la Formulación 3.
3. **La identificación del stakeholder principal correcto** (estudiante), corrigiendo a la IA que puso a Dirección/TI en la F3.
4. **La integración de la Restricción 2** sin caer en juicios de valor, mediante el concepto de "sistemas de sombra".
5. **La distinción entre hecho y supuesto** en la evidencia: la "fuga de capital" quedó marcada como supuesto no cuantificado.

### ¿Qué evidencia del proyecto usó el equipo?

- Enunciado del caso (Restricciones 1, 2 y 3).
- `pestel.md` (factores Tecnológico y Económico argumentados).
- `pestel_evidencias.md` (separación hecho/supuesto).
- `pain-points.md` (análisis de causa raíz: síntomas vs. problemas reales).
- Decisiones humanas ya documentadas (rechazo de "capacitación" y modificación de "sanciones automáticas").

---

## 7. Conexión con las fases anteriores

| Fase | Archivo | Cómo alimentó esta fase |
|---|---|---|
| Stakeholders | `01-stakeholders/stakeholder.md` | Definió los afectados y el stakeholder principal (estudiantes) |
| PESTEL | `02-pestel/pestel.md` + `evidencias.md` | Factores Tecnológico (deuda técnica) y Económico (falsa escasez) dieron el marco de viabilidad |
| Pain Points | `03-pain-points/pain-points.md` | Los 3 problemas raíz fueron la base directa del problema formulado |

**Nota de dependencia:** falta el `stakeholder.md` formal con mínimo 6 stakeholders y la matriz Poder/Interés. Una vez lo entregue el compañero de Fase 1, se debe verificar que el estudiante sea coherentemente el stakeholder principal en ambos documentos.

---

## 8. Conexión con la fase siguiente

### Lean Canvas
Esta formulación alimenta directamente:
- **Bloque "Problema":** los 3 problemas raíz (información, proceso, comunicación).
- **Bloque "Propuesta de valor única":** Single Source of Truth + trazabilidad en tiempo real + alertas automáticas.
- **Bloque "Segmentos de clientes":** estudiantes (primario), docentes, personal de préstamos, dirección.

Si el compañero de Lean Canvas pone algo distinto, deben reunirse y alinear antes de la entrega.

### Defensa oral
Preguntas preparadas:

1. **¿Cuál es la diferencia entre síntoma y problema?**
   → Síntoma: "los estudiantes no devuelven a tiempo" o "aparecen equipos disponibles que están en uso". Problema: "no hay Single Source of Truth ni protocolo de custodia, lo que obliga a improvisar sistemas de sombra".

2. **¿Qué evidencia sostiene este problema?**
   → Restricción 1 del enunciado + `pain-points.md` (problemas raíz) + `pestel.md` (factor Tecnológico). La "fuga de capital" es supuesto, no hecho.

3. **¿Qué propuesta de la IA rechazaron?**
   → La Formulación 2 completa (desalineación operacional). La IA misma la calificó como la más débil. Además, ya tenían documentado el rechazo de "capacitación en software" en `pain-points.md`.

4. **Si desaparece el stakeholder principal, ¿sigue existiendo el problema?**
   → Sí, pero cambia: el personal seguiría con doble registro y la dirección sin datos. El estudiante es el afectado principal, no la causa raíz.

5. **¿Qué parte es supuesto todavía no validado?**
   → La cuantificación de la "fuga de capital" y la existencia de "sistemas de sombra" como práctica generalizada. Requieren entrevistas y observación de campo.

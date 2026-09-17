# IA propone → equipo verifica → evidencia → decisión final

## Decisiones tomadas en Fase 3 (Pain Points)

| Elemento | Propuesta IA | Qué verificamos | Decisión | Razón / evidencia |
|---|---|---|---|---|
| Capacitación del personal | "El pain point del personal operativo es la falta de capacitación en herramientas informáticas" | Contraste con Restricción 2 (desinterés y dispersión de canales) | **RECHAZADA** | El problema es de diseño de proceso y desmotivación, no de competencias. Capacitar no elimina los datos duplicados. |
| Sistema de sanciones | "El problema de los retrasos es la falta de sanciones automáticas a estudiantes" | Análisis de causas en devoluciones | **MODIFICADA** | Los retrasos ocurren por falta de recordatorios y lentitud en la recepción manual, no por falta de castigos. Se reorientó a alertas y agilización. |

## Decisiones tomadas en Fase 4 (Problem/Solution Fit)

| Elemento | Propuesta IA | Qué verificamos | Decisión | Razón / evidencia |
|---|---|---|---|---|
| Formulación 1 (Fragmentación estructural) | "Violación de 3NF y ausencia de Single Source of Truth" | Comprensibilidad para el stakeholder principal + cobertura de Restricción 2 | **MODIFICADA** | Se conservó el núcleo de información, pero se reformuló sin jerga técnica e incorporando la dimensión de proceso |
| Formulación 2 (Desalineación operacional) | "Baja motivación del personal como causa de retrasos" | Coherencia con Restricciones 1 y 2 + evidencia propuesta | **RECHAZADA** | La IA misma la señaló como la más débil. Desvía el problema hacia RR.HH. y no ofrece palanca de ingeniería |
| Formulación 3 (Protocolo de trazabilidad) | "Carencia de protocolo estandarizado de custodia" | Coherencia lógica + stakeholder afectado | **RECHAZADA** | Es tautológica. Malidentifica al stakeholder principal. Su dimensión de proceso se integró a la formulación final |
| Shadow Systems | (No fue propuesta por la IA — la aportó el equipo) | Conexión con Restricciones 1 y 2 | **ADOPTADA parcialmente** | Aporta la causa de la fragmentación: ausencia de canal formal funcional |
| Stakeholder principal | IA: estudiantes (F1), personal (F2), dirección (F3) | Poder/interés + experiencia directa | **Estudiantes** | Sufren la falsa escasez directamente. El personal no sufre el problema |
| Tipo de problema | IA: información+inventario (F1), proceso+comunicación (F2), proceso+información (F3) | Restricciones 1, 2 y 3 | **Información + Proceso + Comunicación** | La información es el núcleo; proceso y comunicación son dimensiones agravantes |

## Propuesta de IA rechazada — declaración formal

**Propuesta rechazada:** Formulación 2 completa — "La brecha entre la urgencia 
operativa de los usuarios solicitantes y la baja motivación del personal de 
préstamos deteriora la ejecución de los protocolos."

**Razón del rechazo:** reduce un problema sistémico de gestión de activos 
tecnológicos a un diagnóstico psicológico o laboral del personal, desviando 
el presupuesto hacia capacitaciones o cambios de actitud en lugar de corregir 
la arquitectura de la información y el proceso de custodia. Además, la propia 
IA la calificó como la más débil de las tres formulaciones que generó.

**Evidencia o razonamiento humano:** la Restricción 2 del caso señala una 
asimetría de interés, no una falta de competencias. El personal no sufre el 
problema; su desinterés sugiere que el estado actual le genera menos fricción 
que adoptar un protocolo estricto. Atacar la actitud no resuelve la 
contradicción de registros (Restricción 1).
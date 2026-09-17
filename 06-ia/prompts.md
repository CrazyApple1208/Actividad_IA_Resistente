# Prompts usados — SQUAD 1

## Prompt 1 — Generar (Ciclo 1)
- **Herramienta:** Gemini
- **Fecha:** [12/09/2026]
- **Propósito:** Generar 3 formulaciones alternativas del problema.
- **Prompt completo:**
Actúa como analista de sistemas crítico, NO como solucionador.



CONTEXTO DEL SISTEMA (SQUAD 1):

Una institución educativa presta computadores portátiles, tabletas, 

proyectores y otros equipos tecnológicos a estudiantes y docentes. 

Actualmente el préstamo se registra mediante formularios, hojas de cálculo 

y mensajes de correo. Existen equipos que aparecen como disponibles aunque 

están siendo utilizados, y otros presentan retrasos en su devolución.



RESTRICCIONES DEL CASO:

1. Un mismo equipo puede aparecer con información diferente en dos registros.

2. El personal encargado no tiene el mismo nivel de interés que los usuarios 

   que solicitan los equipos.

3. El problema principal puede ser de inventario, proceso, información, 

   comunicación o combinación.



HALLAZGOS DEL EQUIPO:



--- PESTEL (factores críticos) ---

Factor Tecnológico: severa deuda técnica y arquitectura de información 

deficiente. Uso de formularios, correos y hojas de cálculo viola integridad 

de datos y normalización (3NF). No existe Single Source of Truth. Hay 

anomalías de actualización: un equipo cambia a "Prestado" en el Excel del 

auxiliar pero sigue "Disponible" en el canal de reservas.

Factor Económico: la ineficiencia genera "falsa escasez" que puede llevar 

a compras injustificadas. El ROI del sistema se justifica si su costo es 

menor que reponer hardware perdido o comprar equipos innecesarios.



--- PAIN POINTS (problemas raíz, no síntomas) ---

1. Descentralización y desfragmentación de la información: no hay Single 

   Source of Truth. Coexisten formularios, hojas de cálculo y correos, 

   generando duplicidad contradictoria (Restricción 1).

2. Alineación operacional y asimetría de interés: brecha entre la necesidad 

   urgente del usuario y la carga/desinterés del personal operativo 

   (Restricción 2).

3. Inexistencia de trazabilidad en tiempo real: falta protocolo unificado 

   para registrar transferencia de custodia de activos.



--- STAKEHOLDERS IDENTIFICADOS ---

- Estudiantes (primario, poder bajo, interés alto)

- Docentes (primario, poder medio, interés alto)

- Personal de préstamos (secundario, poder alto, interés medio)

- Coordinador TI / Dirección (clave, poder alto, interés medio)



--- SÍNTOMAS vs PROBLEMAS (ya diferenciados por el equipo) ---

Síntomas: equipos marcados disponibles pero en uso; retrasos en devolución; 

correos sin responder.

Problemas reales: los 3 pain points raíz listados arriba.



TU TAREA:

Genera 3 formulaciones alternativas del problema para este sistema.

Cada formulación debe explicar QUÉ falla, A QUIÉN afecta y POR QUÉ importa.



Para cada formulación incluye:

- Redacción del problema (máximo 3 líneas)

- Stakeholder principal afectado

- Tipo de problema según restricciones (inventario / proceso / información / 

  comunicación / combinación) y por qué

- Evidencia que necesitaríamos para validarla (NO inventes datos reales)

- Impacto esperado si no se resuelve

- Claridad (alta/media/baja) y por qué

- Relación con el sistema propuesto



REGLAS:

- NO elijas una formulación por nosotros.

- NO inventes cifras ni datos reales.

- Separa HECHOS, SUPUESTOS y RECOMENDACIONES.

- Al final, indícanos qué deberíamos verificar antes de adoptar cualquiera. 



## Prompt 2 — Criticar (Ciclo 2)
- **Herramienta:** Gemini
- **Fecha:** [12/09/2026]
- **Propósito:** Criticar las 3 formulaciones generadas.
- **Prompt completo:
Actúa como revisor crítico de las 3 formulaciones del problema que generaste antes para el sistema de préstamo de equipos tecnológicos.CONTEXTO ORIGINAL:- Institución educativa presta computadores, tabletas, proyectores.- Registro actual: formularios, hojas de cálculo, correos.- Restricción 1: un mismo equipo puede aparecer con info diferente en dos registros.- Restricción 2: el personal encargado no tiene el mismo nivel de interés que los usuarios.- Restricción 3: el problema puede ser de inventario, proceso, información, comunicación o combinación.PROBLEMAS RAÍZ YA VALIDADOS POR EL EQUIPO:1. No hay Single Source of Truth (información desfragmentada).2. Asimetría de interés entre usuarios y personal operativo.3. No hay trazabilidad en tiempo real de la custodia de activos.FACTORES PESTEL CRÍTICOS:- Tecnológico: deuda técnica, arquitectura deficiente, sin 3NF.- Económico: falsa escasez, fuga de capital, ROI justifica el sistema.LAS 3 FORMULACIONES QUE GENERASTE FUERON:

Formulación Alternativa 1: Fragmentación Estructural de la Información

Redacción del problema: La ausencia de una Single Source of Truth y el uso desarticulado de formularios, correos y hojas de cálculo provocan una asimetría crítica en el estado de los equipos, violando la integridad de datos.

Stakeholder principal afectado: Estudiantes y docentes (usuarios primarios con alto interés y bajo/medio poder).

Tipo de problema: Información e inventario (combinación), debido a la falta de normalización (3NF) y anomalías de actualización entre registros dispersos.

Evidencia requerida para validarla: Auditoría de discrepancias temporales entre los registros de los formularios y las hojas de cálculo del auxiliar para un mismo activo tecnológico.

Impacto esperado si no se resuelve: Persistencia de la "falsa escasez" de equipos, generación de compras innecesarias de hardware y pérdida continua de trazabilidad.

Claridad: Alta, ya que la violación de la integridad de datos y la ausencia de una fuente única de verdad están explícitamente documentadas en el análisis tecnológico.

Relación con el sistema propuesto: Evidencia una arquitectura de información deficiente que invalida cualquier intento de control operativo automatizado o manual bajo el esquema actual.

Formulación Alternativa 2: Desalineación Operacional y Asimetría de Interés

Redacción del problema: La brecha entre la urgencia operativa de los usuarios solicitantes y la baja motivación del personal de préstamos deteriora la ejecución de los protocolos, generando retrasos e ineficiencia en la custodia de activos.

Stakeholder principal afectado: Personal de préstamos (secundario, alto poder, interés medio) y los solicitantes (estudiantes/docentes).

Tipo de problema: Proceso y comunicación (combinación), derivada directamente de la asimetría de interés entre los actores involucrados.

Evidencia requerida para validarla: Medición de tiempos de respuesta en correos y análisis de la tasa de cumplimiento de los protocolos de registro por parte del personal operativo.

Impacto esperado si no se resuelve: Aumento sostenido en los retrasos de devolución de equipos y colapso de los canales de comunicación asíncronos (correos sin responder).

Claridad: Media, porque la asimetría de interés es un factor sociotécnico subjetivo que requiere correlación directa con los tiempos de retraso en las devoluciones.

Relación con el sistema propuesto: Demuestra que un cambio meramente tecnológico fallará si no se rediseñan los incentivos y flujos de trabajo del personal encargado de operar el sistema.

Formulación Alternativa 3: Inexistencia de Protocolo de Trazabilidad en Tiempo Real

Redacción del problema: La carencia de un protocolo estandarizado para registrar la transferencia de custodia impide conocer la ubicación real de los dispositivos, generando discrepancias operativas críticas.

Stakeholder principal afectado: Coordinador TI / Dirección (clave, alto poder, interés medio).

Tipo de problema: Proceso e información, al tratarse de una falla metodológica en la captura y actualización del ciclo de vida del activo tecnológico.

Evidencia requerida para validarla: Mapeo del flujo actual de préstamo (desde la solicitud hasta la devolución) para identificar los puntos exactos de pérdida de información y ausencia de validación cruzada.

Impacto esperado si no se resuelve: Incapacidad institucional para auditar el inventario real, aumento del riesgo de pérdida de equipos y justificación errónea de presupuesto para reposición de hardware.

Claridad: Alta, dado que los síntomas directos (equipos disponibles en papel pero en uso físico) son consecuencia directa de este vacío procedimental.

Relación con el sistema propuesto: Expone que el problema no radica únicamente en las herramientas utilizadas (hojas de cálculo), sino en la ausencia de reglas de negocio y procedimientos normalizados para el manejo de los activos.



TU TAREA ES DESTRUIRLAS, NO MEJORARLAS:1. Para cada formulación, señala: - Si confunde SÍNTOMA con PROBLEMA. - Si asume algo que no está en el contexto. - Si ignora alguna de las 3 restricciones. - Si el stakeholder afectado está mal identificado. - Si la evidencia que pide es débil.2. Dime cuál de las 3 es la MÁS DÉBIL y por qué.3. Dime qué formulación alternativa NO consideraste.4. Separa hechos, supuestos y recomendaciones.5. Al final: - ¿Cuál formulación parece más defendible con la evidencia actual? - ¿Qué debería verificar el equipo antes de adoptarla? - ¿Qué propuesta tuya debería rechazar el equipo y por qué?Quiero crítica dura y específica, no balanceada. 











[Pegar aquí el Prompt 2 completo]
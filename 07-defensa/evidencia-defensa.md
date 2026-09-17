# Evidencia de Defensa Oral — SQUAD 1
## Sistema de Préstamos de Equipos Tecnológicos

**Fecha de defensa:** [16/09/2026]
**Integrantes presentes:** CASTELLANOS FORERO JUAN ESTEBAN | PINEDA GONZALEZ JUAN ESTEBAN (SM) | RODRIGUEZ GUARNIZO JERFERSON DAVID | VERGARA PINILLOS JUAN PABLO | VARGAS CARVAJAL JULIAN CAMILO  (PO) 
**Duración:** 5 minutos de pitch + preguntas del docente

---

## 🎤 Guion del pitch (5 minutos)

### Minuto 1 — El problema que consideramos relevante

> "Nuestro squad analizó el sistema de préstamos de equipos tecnológicos de 
> una institución educativa. Después de aplicar los 3 ciclos de IA y 
> contrastar con evidencia del caso, concluimos que el problema **no es de 
> inventario** —hay equipos— sino de **información desfragmentada, proceso 
> sin protocolo y comunicación asimétrica**.
>
> La institución carece de un canal formal único y de una fuente única de 
> verdad para la custodia de los equipos. Esto obliga a usuarios y personal 
> a improvisar 'sistemas de sombra': correos informales, acuerdos verbales 
> y hojas de cálculo paralelas. El resultado: falsa escasez, fricción 
> operativa y decisiones de compra sin datos confiables."

### Minuto 2 — Decisión 1 que cambió después de usar IA

> "La IA nos propuso inicialmente que el problema era la **baja motivación 
> del personal de préstamos**. Decidimos **rechazarla**. La propia IA, en su 
> ciclo de crítica, la calificó como la más débil de sus tres formulaciones. 
> Reducir un problema sistémico a un diagnóstico actitudinal desvía el 
> presupuesto hacia capacitaciones en lugar de corregir la arquitectura de 
> la información y el proceso de custodia."

### Minuto 3 — Decisión 2 que cambió después de usar IA

> "La IA también propuso un **sistema de sanciones automáticas** para 
> estudiantes que devolvieran tarde. Decidimos **modificarla**: los retrasos 
> no ocurren por falta de castigos, sino por ausencia de alertas automáticas 
> y por la lentitud del registro manual de recepción. Reorientamos el enfoque 
> hacia notificaciones automáticas y agilización del proceso de devolución."

### Minuto 4 — Stakeholder que inicialmente omitimos o clasificamos mal

> "La IA clasificó al personal de préstamos como 'interés alto'. Nosotros lo 
> **modificamos a interés medio**. El personal no busca beneficiarse del 
> sistema; su interés es defensivo: evitar que le aumente la carga. Esto 
> cambió la estrategia de gestión: pasamos de 'mantener satisfecho' a 
> 'mantener informado y gestionar el cambio'."

### Minuto 5 — Incoherencia detectada en el Lean Canvas

> "Detectamos una incoherencia: el bloque 'Canales' incluía una app móvil, 
> pero el stakeholder primario (estudiantes) tiene bajo poder de decisión y 
> la institución no ha validado presupuesto para desarrollo móvil. 
> **Corregimos**: el canal principal es el portal web institucional; la app 
> móvil queda como fase 2."

---

## 📋 Banco de preguntas de defensa — Respuestas preparadas

### 1. ¿Por qué este stakeholder tiene ese nivel de poder y no otro?

**Stakeholder:** Estudiantes — Poder **bajo**, Interés **alto**.

**Respuesta:**
> Los estudiantes tienen poder bajo porque no deciden la compra, la 
> asignación ni las políticas de préstamo; solo solicitan el servicio. Su 
> interés es alto porque dependen directamente del equipo para sus clases y 
> entregas académicas. El poder de decisión está en la Dirección y el 
> Coordinador TI, pero el dolor operativo lo sufre el estudiante.

**Evidencia:** `pain-points.md` + `stakeholder.md` + Restricción 2 del caso.

---

### 2. ¿Qué evidencia tienen para afirmar que este pain point es real?

**Pain point:** Incertidumbre en la disponibilidad del equipo.

**Respuesta:**
> La evidencia principal está en el enunciado del caso (Restricción 1): 
> *"un mismo equipo puede aparecer con información diferente en dos 
> registros"*. Esto significa que el estudiante puede llegar al mostrador y 
> encontrar que el equipo que el sistema marcaba como disponible está en uso. 
> Además, el caso confirma textualmente que existen *"equipos que aparecen 
> como disponibles aunque están siendo utilizados"*.

**Evidencia:** Enunciado del caso + `pain-points.md` (problema raíz #1) + 
`pestel_evidencias.md` (factor Tecnológico, hecho comprobado).

---

### 3. ¿Cuál de sus stakeholders podría bloquear el proyecto?

**Respuesta:**
> El **personal de préstamos**. Es el stakeholder con poder alto e interés 
> medio. Si el sistema les aumenta la carga operativa o no les facilita el 
> trabajo, pueden resistirse a usarlo y boicotearlo pasivamente. La 
> Restricción 2 del caso señala explícitamente esta asimetría de interés. 
> Por eso la estrategia de gestión es "mantener satisfecho" y gestionar el 
> cambio, no solo capacitarlos.

**Evidencia:** Restricción 2 + `stakeholder.md` + `pain-points.md`.

---

### 4. ¿Qué propuesta de la IA rechazaron y por qué?

**Respuesta:**
> Rechazamos la **Formulación 2** de la IA: *"La brecha entre la urgencia 
> operativa de los usuarios y la baja motivación del personal deteriora la 
> ejecución de los protocolos"*. La rechazamos porque:
>
> 1. La propia IA la calificó como la más débil de sus tres formulaciones.
> 2. Reduce un problema sistémico a un juicio de valor sobre la actitud del personal.
> 3. Ignora la Restricción 1 (contradicción de registros).
> 4. Propone evidencia débil: medir tiempos de correo es métrica de desempeño individual, no evidencia sistémica.

**Evidencia:** `06-ia/decisiones-humanas.md` + `salidas-ia.md` (crítica de la IA).

---

### 5. ¿Qué parte de su análisis es un supuesto todavía no validado?

**Respuesta:**
> Dos supuestos principales:
>
> 1. **La "fuga de capital" por falsa escasez.** Asumimos que la 
>    ineficiencia genera compras innecesarias, pero no tenemos cifras 
>    reales de cuánto gasta la institución en reposición de hardware.
> 2. **La existencia generalizada de "sistemas de sombra".** Inferimos que 
>    usuarios y personal improvisan canales informales, pero no lo hemos 
>    observado directamente ni cuantificado.
>
> Ambos requieren entrevistas al área financiera y observación de campo.

**Evidencia:** `pestel_evidencias.md` (columna "Supuesto por validar") + 
`problem-solution-fit.md` (sección 1.3).

---

### 6. ¿Qué factor PESTEL podría cambiar la viabilidad de su sistema?

**Respuesta:**
> El **factor Tecnológico** (infraestructura de red). Asumimos que la 
> institución cuenta con servidores y conectividad estable para soportar 
> peticiones concurrentes a una base de datos centralizada, especialmente 
> durante picos de inicio y fin de semestre. Si esa infraestructura no 
> existe, el sistema tendría que rediseñarse como una solución local o 
> híbrida, y el ROI cambiaría radicalmente.
>
> También el **factor Legal**: la Ley 1581 de 2012 exige manejo seguro de 
> datos personales. Si la institución no tiene política interna de 
> protección de datos, el sistema debe incluirla o no puede desplegarse.

**Evidencia:** `pestel.md` (factores Tecnológico y Legal) + 
`pestel_evidencias.md` (supuesto de infraestructura).

---

### 7. ¿Cuál es la diferencia entre el síntoma y el problema que identificaron?

**Respuesta:**
> **Síntoma:** *"los estudiantes no devuelven a tiempo"* o *"aparecen 
> equipos disponibles que están en uso"*. Estas son manifestaciones visibles.
>
> **Problema raíz:** *"no hay Single Source of Truth ni protocolo de custodia, 
> lo que obliga a improvisar sistemas de sombra"*. Esta es la causa que 
> origina los síntomas.
>
> Si solo atacamos el síntoma (ej. sancionar a estudiantes), no resolvemos 
> nada. Si atacamos el problema raíz (centralizar información y protocolizar 
> la custodia), los síntomas disminuyen como consecuencia.

**Evidencia:** `pain-points.md` (sección 1 — Síntomas vs. Problemas reales).

---

### 8. ¿Qué bloque del Lean Canvas depende más directamente del stakeholder primario?

**Respuesta:**
> El bloque **"Propuesta de Valor Única"** y el bloque **"Canales"**.
>
> La propuesta de valor —*"estado en tiempo real de cada equipo y 
> trazabilidad por responsable"*— responde directamente a la necesidad del 
> estudiante: saber si el equipo está disponible antes de solicitarlo.
>
> El canal principal (portal web institucional) también depende del 
> estudiante: debe ser accesible, rápido y comprensible. Si el canal no le 
> sirve al estudiante, el sistema no se adopta.

**Evidencia:** `05-lean-canvas/lean-canvas.png` + 
`problem-solution-fit.md` (sección 3).

---

### 9. Si desapareciera el stakeholder principal, ¿seguiría existiendo el problema?

**Respuesta:**
> **Sí, pero cambiaría de forma.** El personal seguiría con doble registro 
> manual y la dirección seguiría sin datos consolidados para decidir compras. 
> El problema raíz (falta de Single Source of Truth y de protocolo de 
> custodia) no depende de la existencia del estudiante.
>
> Sin embargo, la **urgencia** del problema bajaría, porque el estudiante es 
> quien sufre la falsa escasez directamente. Sin él, el problema sería más 
> silencioso: solo lo notarían TI y Financiera en los reportes.

**Evidencia:** `problem-solution-fit.md` (sección 2 — Afectados).

---

### 10. ¿Qué decisión tomó el equipo que la IA no podía tomar por ustedes?

**Respuesta:**
> Tres decisiones clave:
>
> 1. **Identificar al estudiante como stakeholder principal**, no al 
>    personal de préstamos ni a la Dirección. La IA en su Formulación 3 
>    puso a la Dirección como principal afectado; el equipo corrigió.
> 2. **Rechazar la Formulación 2** completa, a pesar de que la IA la generó 
>    como alternativa válida. La IA no podía saber que el equipo ya había 
>    documentado en `pain-points.md` un rechazo similar (capacitación del 
>    personal).
> 3. **Integrar el concepto de "sistemas de sombra"**, que la IA no propuso 
>    en su primera generación. El equipo lo detectó como la pieza que 
>    conectaba las Restricciones 1 y 2.

**Evidencia:** `06-ia/decisiones-humanas.md` (tabla completa).


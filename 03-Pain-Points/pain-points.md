FASE 3: DETECCIÓN DE PAIN POINTS REALES 
 
1. ANÁLISIS DE CAUSA RAÍZ: SÍNTOMAS VS. PROBLEMAS REALES 
 
Para enfocar el desarrollo del sistema en lo que realmente aporta valor y no en simples manifestaciones superficiales, se analizaron las causas raíz del problema: 
 
Síntomas (Manifestaciones visibles): 


Equipos que figuran como "disponibles" en el registro, pero están prestados o no se encuentran físicamente. 

Retrasos recurrentes en las devoluciones de computadores portátiles, tabletas y proyectores. 

Correos de solicitud sin responder, traspapelados o con respuestas tardías. 
 
Problemas Reales (Causa Raíz Operacional y de Información): 


Descentralización y Desfragmentación de la Información: Inexistencia de una Única Fuente de Verdad (Single Source of Truth). La coexistencia de formularios, hojas de cálculo y correos electrónicos rompe la integridad de los datos y genera duplicidad contradictoria (Restricción #1). 

Alineación Operacional y Asimetría de Interés: Brecha entre la necesidad urgente del usuario (estudiante/docente) y la carga/desinterés del personal operativo encargado de la entrega y recepción (Restricción #2). 

Inexistencia de Trazabilidad en Tiempo Real: Falta de un protocolo unificado y automatizado para registrar la transferencia de custodia de los activos tecnológicos al momento de la entrega o devolución. 


2. MATRIZ DE PAIN POINTS Y TABLA DE TRAZABILIDAD (pain-points.md) 

Stakeholder: Usuarios (Estudiantes / Docentes) 
 
Tipo / Rol: Primarios 
 
Pain Point Principal (Problema Real): Incertidumbre en la disponibilidad. La información desactualizada no garantiza tener el equipo a tiempo para clases, laboratorios o entregas académicas. 
 
Impacto / Evidencia: Frustración, pérdida de horas de clase, actividades preparadas canceladas y entregas extemporáneas. 
 
Decisión del Equipo: Conservar (Impacto directo en los usuarios finales del servicio). 
 
Stakeholder: Operadores (Personal de préstamos) 
 
  	Tipo / Rol: Secundarios 
 
Pain Point Principal (Problema Real): Fricción por procesos manuales 	dispersos. Carga administrativa alta manejando correo, papel y Excel de forma paralela (Restricción #2). 
 
Impacto / Evidencia: Carga laboral, alta tasa de error humano, desmotivación 	y tensión frecuente con los usuarios. 
 
 	Decisión del Equipo: Conservar (Explica la causa raíz del desinterés y los 	   	registros duplicados). 
 
Stakeholder: Directivos (Coordinador TI / Dirección) 
 
  	Tipo / Rol: Clave 
 
Pain Point Principal (Problema Real): Pérdida de trazabilidad y control de 	  activos. Datos contradictorios sobre ubicación, estado y uso real de los equipos (Restricción #1).


Impacto / Evidencia: Pérdida de hardware, gastos innecesarios en compras 	de sustitución y fallas en ciclos de mantenimiento. 
 
Decisión del Equipo: Conservar (Justifica técnicamente la inversión en el 	nuevo sistema).


3. EVIDENCIA DEL USO DE IA NIVEL 3 (decisiones-humanas.md) 
 
Prompt ejecutado (Ciclo 1 - Generar): 
"Actúa como analista de sistemas crítico. A partir del caso de 			préstamos de equipos académicos con registros contradictorios y 			desinterés del personal operativo, genera 5 pain points para los 			stakeholders. Diferencia síntomas de problemas reales." 
 
Análisis Crítico de Propuestas de IA (Ciclos 2 y 3: Criticar y Decidir) 
 
1. Propuesta de IA Rechazada (Capacitación del personal): 
 
Propuesta de IA: "El Pain Point del personal operativo es la falta de capacitación en herramientas informáticas para inventarios." 
 
Decisión: RECHAZAR. 
 
Justificación Humana: La Restricción #2 del caso señala explícitamente un problema de desinterés y dispersión de canales (Excel, correo, papel), no de falta de competencias informáticas. Capacitarlos en hojas de cálculo no elimina la inconsistencia de registros duplicados ni la desalineación de procesos. 
 
2. Propuesta de IA Modificada (Sistema de sanciones): 
 
Propuesta de IA: "El problema principal de los retrasos en devoluciones es la falta de un sistema de sanciones o multas automáticas para los estudiantes." 
 
Decisión: MODIFICAR.
 
Justificación Humana: Los retrasos en devoluciones no ocurren principalmente por mala fe o falta de castigos, sino por la ausencia de alertas/recordatorios automáticos y por la lentitud del registro manual de recepción por parte del personal. Se ajustó el enfoque hacia la automatización de notificaciones y la agilización de la recepción en lugar de un módulo punitivo.

Registro Consolidado de Decisión Humana (decisiones-humanas.md):
 
Propuesta de la IA: "El personal operativo requiere capacitaciones en software de inventarios."
 
Verificación frente al Caso: Contraste con la Restricción #2 (desinterés y dispersión de canales).
 
  	Decisión: RECHAZAR.
 
  	Razón / Evidencia Humana: El problema es de diseño de proceso y falta        de motivación. Capacitarlos no elimina los datos duplicados. 
 
Propuesta de la IA: "El problema central es la falta de sanciones automáticas 	a los estudiantes." 
 
  	Verificación frente al Caso: Análisis de causas en devoluciones. 
  	Decisión: MODIFICAR. 
 
Razón / Evidencia Humana: Los retrasos ocurren por falta de recordatorios   y lentitud en la recepción manual, no por falta de castigos.







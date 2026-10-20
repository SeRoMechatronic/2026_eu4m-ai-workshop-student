# Mapa de aplicaciones de IA en mecatrónica

La mecatrónica integra cuatro disciplinas. Cada una ya tiene aplicaciones de IA
en la industria, con la misma regla en las cuatro: una salida útil todavía
necesita una prueba independiente antes de confiar en ella en un sistema real.
El caso del actuador del módulo 3 profundiza en control y diagnóstico; esta
página sitúa ese caso dentro del panorama completo.

## Electrónica

- **Asistencia al diseño de PCB:** sugerencias de colocación de componentes y
  enrutado asistido por IA en herramientas EDA, y respuesta a preguntas sobre
  hojas de datos.
- **Inspección óptica automática (AOI):** modelos de aprendizaje automático
  detectan defectos de soldadura o componentes mal colocados en la línea de
  producción.
- **Qué verificar:** la tasa de falsos positivos y falsos negativos del
  clasificador en su propio proceso, no en el dataset de validación del
  proveedor. Un detector de defectos no auditado puede aprobar una placa
  defectuosa o rechazar una buena.

## Mecánico

- **Diseño generativo y optimización topológica:** herramientas como Autodesk
  Fusion, Siemens NX, PTC Creo GDX, Altair Inspire o nTopology proponen
  geometrías que cumplen cargas y restricciones con menos material.
- **Modelos sustitutos de FEA y CFD:** aceleran la iteración de diseño con una
  aproximación entrenada, antes de una simulación completa de validación.
- **Qué verificar:** las cifras de ahorro de material o tiempo que publican los
  fabricantes son casos de demostración propios, no una medición independiente
  en su aplicación. La geometría generada normalmente necesita convertirse a un
  sólido paramétrico editable antes de pasar a fabricación.

## Control

- **Diagnóstico de fallos basado en datos:** el mismo problema que trabaja el
  caso del actuador del módulo 3, a mayor escala: modelos de residuos y
  aprendizaje automático comparan comportamiento observado con el esperado
  (Isermann, 2005; Lei et al., 2020).
- **Ajuste de controladores con aprendizaje por refuerzo:** cada vez más
  explorado en investigación, pero el ajuste clásico de un controlador incluye
  una fase de verificación física que el entrenamiento por refuerzo en
  simulación normalmente omite. Un estudio con un octorrotor encontró que la
  desviación en vuelo real llegó a duplicar la de simulación.
- **Qué verificar:** cualquier controlador o detector entrenado en simulación
  necesita una medición independiente en el sistema real antes de confiar en
  él, exactamente la lección del módulo 3 sobre `position_true_m`.

## Programación

- **Asistentes de código para sistemas embebidos:** generan firmware de
  arranque, controladores de periféricos y pruebas. Una compilación limpia
  confirma sintaxis y enlazado, no temporización, gestión de interrupciones ni
  comportamiento del hardware real.
- **Dónde falla con más frecuencia:** temporización por interrupciones,
  concurrencia y orden de acceso a datos compartidos.
- **Qué verificar:** pruebas en hardware representativo además de análisis
  estático y revisión humana; reserve el código generado para tareas de menor
  riesgo (andamiaje, documentación, pruebas) y revise con más rigor el código de
  temporización crítica o lógica de seguridad.

## La misma pregunta en las cuatro disciplinas

Antes de aceptar una salida de IA en cualquiera de estas áreas, pregunte: ¿qué
mediría en el sistema real, independiente de la herramienta, para confirmar o
refutar esto? Si no puede responder, la salida queda pendiente, no aceptada.

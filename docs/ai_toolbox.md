# Caja de herramientas de IA para investigación y escritura

Estas herramientas son opcionales y ninguna es obligatoria para completar el curso.
El método que se evalúa es PVRD, no el uso de una herramienta concreta. La
coordinación de la Universidad decide qué cuentas y servicios están autorizados
([tool_policy.md](tool_policy.md)); verifique antes de instalar o registrarse con
un correo institucional.

Las condiciones de acceso, precio y funciones de estas herramientas cambian con
frecuencia. Las cifras de esta página se comprobaron el 20 de octubre de 2026 y
el docente debe revisarlas antes de cada nueva edición del curso.

## Gestión de referencias

### Zotero

Gestor de referencias gratuito y de código abierto. Captura metadatos desde el
navegador, organiza PDF y genera citas y bibliografía en el estilo que necesite.

- **Para qué sirve aquí:** sustituye copiar referencias a mano en la matriz de
  fuentes; el conector de navegador reduce errores de transcripción de autor,
  año y título.
- **Verifique siempre:** que el conector capturó el DOI correcto, no solo un
  título parecido. Zotero importa lo que encuentra en la página; no confirma que
  el metadato sea exacto.
- **Límite conocido:** el almacenamiento gratuito en la nube se limita a 300 MB
  para archivos adjuntos; los PDF pueden mantenerse en local sin ese límite.

## Descubrimiento de literatura con lenguaje natural

### Elicit

Asistente de investigación que permite describir una pregunta en lenguaje
natural y obtener artículos, resúmenes generados y extracción de datos a tablas
comparables. Cada celda de la tabla puede enlazar a la frase exacta del artículo
de la que procede.

- **Para qué sirve aquí:** acelera el cribado inicial de una pregunta amplia.
- **Verifique siempre:** la frase enlazada en el artículo original, no solo el
  resumen generado.
- **Límite conocido y ejemplo de auditoría:** Elicit publicó una sensibilidad del
  96,9 % para su cribado de resúmenes en 994 revisiones Cochrane. Un estudio
  independiente (Lau et al., 2025) encontró que la sensibilidad caía a 37,9 %
  cuando se aplicaban estrategias de búsqueda reales de revisión sistemática.
  **Este es el ejemplo que se audita en el módulo 2**: la cifra que publica la
  propia herramienta no basta como evidencia de su fiabilidad.

### Undermind

Agente de búsqueda que no empareja palabras clave: explora cientos de artículos
de forma iterativa, sigue cadenas de citas y explica por qué cada resultado
coincide con la pregunta.

- **Para qué sirve aquí:** encontrar trabajos relevantes que una búsqueda por
  palabras clave pasaría por alto.
- **Verifique siempre:** por qué el sistema considera relevante cada resultado;
  la explicación generada es también una afirmación que auditar.
- **Límite conocido:** la comparación de un 10× más de resultados relevantes
  frente a Google Scholar procede de un informe técnico de la propia empresa;
  no es una evaluación independiente.

## Verificar el respaldo de una cita

### scite.ai

Clasifica cada cita de un artículo como que respalda, contradice o solo
menciona el trabajo citado, y muestra la frase exacta donde ocurre la cita.

- **Para qué sirve aquí:** distinguir una cita decorativa de una que realmente
  aporta evidencia a favor o en contra, antes de usarla en la matriz de fuentes.
- **Verifique siempre:** lea la frase mostrada, no solo la etiqueta. La
  clasificación es un indicio, no una lectura del pasaje.
- **Límite conocido:** la propia scite reporta una precisión del 97 % para
  "menciona", pero de solo 64 % para "respalda" y 59 % para "contradice". Las
  categorías con más valor para el curso son las menos fiables.

### Consensus

Busca en un índice amplio de literatura académica y sintetiza con citas lo que
encuentra; el "Consensus Meter" muestra si los artículos recuperados coinciden,
discrepan o se dividen sobre una pregunta de sí/no.

- **Para qué sirve aquí:** una primera panorámica de si una afirmación tiene
  respaldo amplio o es controvertida.
- **Verifique siempre:** cuántos artículos analizó realmente el modo usado (los
  modos rápidos analizan muy pocos) y si esos artículos responden a la pregunta
  concreta del curso, no solo al tema general.
- **Límite conocido:** el indicador de consenso resume el sentido de los
  artículos recuperados, no mide la calidad metodológica de cada uno.

## Síntesis sobre su propio corpus

### NotebookLM

Asistente que responde solo a partir de los documentos que usted sube (PDF,
páginas web, apuntes), y está diseñado para declinar cuando la respuesta no
está respaldada por esas fuentes.

- **Para qué sirve aquí:** preguntar sobre sus propias fuentes ya verificadas sin
  mezclar conocimiento general del modelo.
- **Verifique siempre:** que la cita que acompaña la respuesta señale el pasaje
  correcto dentro de su documento, no un fragmento relacionado pero distinto.
- **Límite conocido:** anclar la respuesta a sus fuentes ("grounding") limita de
  dónde viene la respuesta, pero no garantiza que la respuesta sea correcta.
  Reduce un riesgo (inventar una fuente) y deja abierto otro (interpretar mal la
  fuente real).

## Regla general para cualquier herramienta nueva

Antes de confiar en una herramienta que no está en esta lista, aplique PVRD a la
herramienta misma: qué afirma hacer, qué prueba independiente de esa afirmación
existe, qué se corrige si falla y dónde queda registrado. El caso de Elicit de
esta página es la plantilla.

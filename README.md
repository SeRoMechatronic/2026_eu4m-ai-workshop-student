# IA aplicada con verificación · Material del estudiante

Curso presencial de 8 horas para estudiantes de primer semestre de EU4M
(Universidad de Oviedo). Cada uso relevante de inteligencia artificial sigue el
protocolo **PVRD**:

1. **Prompt**: definir propósito, contexto y criterio de aceptación.
2. **Verificar**: contrastar la salida con una fuente, cálculo, prueba o dato.
3. **Refinar**: corregir la salida o reformular la petición.
4. **Documentar**: registrar la decisión, los cambios y los límites.

## Antes de la primera sesión (5 minutos)

1. Lea la [guía del estudiante](docs/student_guide.md).
2. Abra la **comprobación de acceso** en Colab:
   [Abrir 00_access_check.ipynb](https://colab.research.google.com/github/SeRoMechatronic/2026_eu4m-ai-workshop-student/blob/main/notebooks/00_access_check.ipynb)
   y pulse *Entorno de ejecución → Ejecutar todo*.
3. Envíe al docente la línea que empieza por `ACCESO_OK`. Si algo falla, envíe una
   captura de pantalla y no instale nada por su cuenta.

Colab necesita una cuenta de Google. Si su cuenta institucional no permite Colab,
avise antes de la sesión: trabajará en pareja o con el material sin conexión.

## Durante el curso

Este repositorio se publica **módulo a módulo**, según avanza el curso: el
material de una sesión aparece aquí poco antes de impartirse. Si busca un
enunciado y `activities/` todavía no lo tiene, es que su módulo aún no empezó.

- Cada módulo trae su propio enunciado en `activities/` y, si corresponde, un
  notebook o un documento de referencia enlazado desde ese mismo enunciado.
- Plantillas, disponibles desde el primer día: [registro PVRD](templates/pvrd_log.csv),
  [matriz de fuentes](templates/source_matrix.csv),
  [informe técnico](templates/engineering_brief.md) y
  [declaración de uso de IA](templates/ai_use_declaration.md).
- Los archivos del reto del módulo 4 se entregan durante la sesión, no por el
  repositorio.
- Conserve todas sus evidencias hasta el cierre del curso.

## Ejecución local (opcional)

Requiere Python 3.10 o posterior.

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
jupyter notebook notebooks/03_actuator_case_student.ipynb
```

## Contenido

| Ruta | Contenido |
|---|---|
| `docs/` | Programa, guía del estudiante, política de herramientas y referencias; cada módulo añade su propio documento al publicarse |
| `activities/` | Enunciado de cada módulo ya publicado |
| `templates/` | Entregables editables, disponibles desde el primer día |
| `notebooks/` | Comprobación de acceso desde el primer día; el notebook de un módulo técnico se añade al publicarse |
| `data/` | Datos sintéticos por escenario y metadatos con huellas SHA-256 |
| `src/` | Código del simulador, para lectura y reproducción |

## Límites del caso técnico

El actuador es un modelo sintético de una masa controlada por PD. Sirve para
enseñar verificación, diseño de pruebas y razonamiento sobre fallos. No representa
un actuador industrial concreto y sus resultados no deben presentarse como
validación de un sistema de diagnóstico real.

## Datos y privacidad

No cargue datos personales, confidenciales o sujetos a acuerdos de proyecto en
herramientas externas. Consulte la [política de herramientas](docs/tool_policy.md).

## Licencias

- Código: licencia MIT ([LICENSE-CODE](LICENSE-CODE)).
- Guías, actividades y plantillas: Creative Commons Attribution 4.0
  ([LICENSE](LICENSE)).
- Las publicaciones citadas mantienen sus licencias originales.

## Autor

José Sebastián Rojas Ordóñez  
Antiguo alumno de EU4M  
Investigador predoctoral en IKERLAN y University of the Basque Country (UPV/EHU)

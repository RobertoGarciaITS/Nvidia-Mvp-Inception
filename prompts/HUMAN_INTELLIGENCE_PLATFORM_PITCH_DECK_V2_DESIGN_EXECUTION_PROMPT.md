# Design Execution Prompt — Human Intelligence Platform Pitch Deck v2

## Rol

Actúa como director de producto, arquitecto de información, diseñador UX/UI de presentaciones y editor de pitch decks para NVIDIA Inception. Produce una versión 2 del pitch deck de Human Intelligence Platform utilizando exclusivamente la arquitectura aprobada y el contrato de contenido.

## Fuentes obligatorias

Lee primero:

1. `governance/PROJECT_SCOPE_v0.1.md`
2. `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_CONTRACT_v0.1.json`
3. `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json`
4. `contracts/architecture/DIGITAL_TWIN_MATURITY_CONTRACT_v0.1.json`
5. `contracts/architecture/HUMAN_INTELLIGENCE_PLATFORM_LIFE_DOMAINS_CONTRACT_v0.1.json`
6. `contracts/presentation/HUMAN_INTELLIGENCE_PLATFORM_PITCH_DECK_V2_CONTENT_DESIGN_CONTRACT_v0.1.json`
7. `docs/presentation/HUMAN_INTELLIGENCE_PLATFORM_PITCH_DECK_V2_CONTENT_PLAN.md`

## Objetivo

Crear un deck de 16 diapositivas que explique:

> Human Intelligence Platform es una plataforma Human-in-the-Loop Digital Twin para que las personas gestionen su Gemelo Digital Personal y las organizaciones gestionen su Gemelo Digital Empresarial, conectados mediante relaciones autorizadas para producir progreso medible y verificable.

El estudiante es el primer beachhead provisional. La arquitectura integral Personal + Enterprise es el destino del producto. No presentes la arquitectura objetivo como una funcionalidad ya implementada.

## Formato obligatorio de cada diapositiva

Para cada una de las 16 diapositivas genera exactamente estos campos:

`slide_id`, `order`, `slide_type`, `title`, `context`, `data`, `bullets`, `body_copy`, `visual_type`, `chart_series`, `chart_format`, `claim_status`, `source_or_evidence`, `design_status`, `speaker_note`.

Cada dato debe incluir valor, unidad si aplica, status y source. Si no existe dato cuantitativo, usa `null` y explica por qué. Si no hay una gráfica cuantitativa, usa `chart_series: []` y describe el diagrama editable en `chart_format`.

## Instrucciones de contenido

- Usa los 16 registros del contrato sin cambiar su orden.
- Conserva la diferencia entre Personal Digital Twin, Enterprise Digital Twin y Authorized Relationship Layer.
- Incluye los siete dominios personales y los siete dominios empresariales.
- Incluye People Twins, Asset Twins, Process Twins y Product Twins como twins anidados dentro del Enterprise Twin.
- Explica que un perfil de usuario no es un Digital Twin completo.
- Incluye el modelo de madurez M0 a M6.
- Presenta M3 como objetivo mínimo y M6 como visión de federación de twins.
- Presenta el estudiante como hipótesis de beachhead, no como mercado validado.
- Mantén la frontera del MVP: identidad, consentimiento, Human Twin Core, eventos, evidencia, capacidades, un dominio y un agente.
- No inventes métricas, clientes, usuarios, ingresos, benchmarks, partners ni afiliación NVIDIA.

## Instrucciones de diseño

- Usa diagramas editables para arquitectura, relaciones, ciclos y roadmaps.
- Usa una gráfica cuantitativa sólo cuando exista una serie numérica real.
- No uses una matriz de tarjetas como sustituto de una arquitectura.
- No uses logos como decoración.
- Mantén una composición limpia, con una idea dominante por diapositiva.
- Usa títulos directos y texto breve, profesional y verificable.
- Conserva los placeholders como `TBD`, `PENDING` o `TO_VALIDATE`.

## Validación previa a la entrega

1. Existen exactamente 16 diapositivas.
2. Cada diapositiva contiene los 15 campos requeridos.
3. Cada afirmación tiene estado y fuente.
4. Cada número tiene unidad, fecha y fuente.
5. No se presenta la arquitectura como implementación.
6. El MVP y la visión de largo plazo están separados.
7. Los placeholders de piloto, benchmark, inversión y equipo no se convierten en hechos.
8. El deck responde qué hace la plataforma, para quién empieza, cómo funciona, cómo madura y qué evidencia falta.

## Entregables

- Especificación completa de contenido para 16 diapositivas.
- Plan visual por diapositiva.
- Texto visible de cada diapositiva.
- Notas del presentador con caveats y estado de evidencia.
- Matriz final de pendientes.
- Lista de afirmaciones que requieren validación antes de una versión final para NVIDIA Inception.

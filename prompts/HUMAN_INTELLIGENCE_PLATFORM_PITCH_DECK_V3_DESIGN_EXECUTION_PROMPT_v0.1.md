# Design Execution Prompt — Human Intelligence Platform Pitch Deck v3

## Rol

Actúa como director de producto, arquitecto de información, diseñador UX/UI de presentaciones y editor de pitch decks para NVIDIA Inception. Produce una versión v3 de Human Intelligence Platform usando como fuente principal el contrato v3.0.3.

## Fuente principal obligatoria

Lee primero el contrato completo:

`contracts/presentation/HUMAN_INTELLIGENCE_PLATFORM_PITCH_DECK_V3_CONTENT_DESIGN_CONTRACT_v0.3.json`

Después lee las fuentes de arquitectura y gobernanza:

1. `AGENTS.md`
2. `README.md`
3. `governance/PROJECT_SCOPE_v0.1.md`
4. `governance/VARIABLE_REGISTRY_v0.1.json`
5. `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_CONTRACT_v0.1.json`
6. `contracts/architecture/PERSONAL_ENTERPRISE_DIGITAL_TWIN_ARCHITECTURE_CONTRACT_v0.2.json`
7. `contracts/architecture/DIGITAL_TWIN_MATURITY_CONTRACT_v0.1.json`
8. `contracts/architecture/HUMAN_INTELLIGENCE_PLATFORM_LIFE_DOMAINS_CONTRACT_v0.1.json`
9. `docs/NVIDIA_INCEPTION_PREFLIGHT_PROGRESS.md`
10. `docs/presentation/HUMAN_INTELLIGENCE_PLATFORM_PITCH_DECK_V2_CONTENT_PLAN.md`

## Objetivo

Crear un deck de 19 diapositivas que explique:

> Human Intelligence Platform es una plataforma Human-in-the-Loop Digital Twin para que las personas gestionen su Personal Digital Twin y las organizaciones gestionen su Enterprise Digital Twin, conectados mediante Authorized Relationship Layer para producir progreso medible y verificable.

El modelo de negocio se presenta como hipótesis integral:

```text
B2C — Personal Digital Twin
B2E — Enterprise Digital Twin
B2B — Authorized Digital Twin relationships
```

El estudiante aparece únicamente como el primer beachhead B2C provisional. No representa el mercado completo ni el alcance integral de la plataforma.

## Secuencia obligatoria

1. Tesis integral
2. Contexto humano y organizacional fragmentado
3. Why now
4. Personal Twin, Enterprise Twin y relaciones autorizadas
5. Loop operativo del Digital Twin
6. Human Twin Core
7. Evidence Graph
8. Capability Graph
9. Personal Digital Twin: siete dominios
10. Enterprise Digital Twin: dominios y twins anidados
11. Authorized Relationship Layer
12. Permissioned AI Agents and Human Decisions
13. Trust and Governance
14. Verified Human Progress
15. One Beachhead, One Decision, One Evidence Loop
16. Digital Twin Maturity
17. NVIDIA Technical Workloads
18. Roadmap and Evidence Gates
19. Founder, Team and Ask

## Formato obligatorio de cada diapositiva

Para cada una de las 19 diapositivas usa exactamente los campos del contrato:

`slide_id`, `order`, `slide_type`, `title`, `context`, `data`, `bullets`, `body_copy`, `visual_type`, `chart_series`, `chart_format`, `claim_status`, `source_or_evidence`, `design_status`, `speaker_note`.

Cada dato debe incluir valor, unidad si aplica, status y source. Si no existe dato cuantitativo, usa `chart_series: []` y describe el diagrama editable en `chart_format`.

## Reglas de contenido

- Conserva la separación entre Personal Digital Twin, Enterprise Digital Twin y Authorized Relationship Layer.
- Incluye los siete dominios personales como modelo organizativo propuesto, no como implementación completa.
- Incluye los dominios empresariales y People, Asset, Process y Product Twins como arquitectura propuesta.
- Explica que un perfil no es un Digital Twin completo.
- Incluye el modelo de madurez M0 a M6, con M3 como objetivo mínimo y M6 como visión federada.
- Mantén el MVP limitado a Identity, Consent, Human Twin Core, Events, Evidence Graph, Capability Graph, one Domain View y one Agent.
- Presenta AI Agents como asistentes de contexto autorizado, nunca como fuentes de verdad ni autoridad automática.
- Presenta Verified Human Progress como north star, no como tracción demostrada.
- Mantén los campos de piloto, benchmarks, equipo, inversión y partners como `TBD`, `PENDING` o `TO_VALIDATE` cuando falte evidencia.
- No inventes clientes, usuarios, ingresos, benchmarks, partners, mercado, afiliación NVIDIA o resultados.

## Reglas de diseño

- Usa diagramas editables para arquitectura, relaciones, ciclos, grafos y roadmap.
- Usa gráficas cuantitativas sólo con series reales, unidad, fecha y fuente.
- No uses dashboards o matrices de tarjetas como sustituto de una arquitectura.
- No uses logos NVIDIA como decoración.
- Mantén una idea dominante por diapositiva.
- Usa títulos directos y texto breve, profesional y verificable.
- Distingue visualmente hechos, hipótesis, arquitectura propuesta y pendientes.
- Mantén suficiente tamaño de texto para presentación y evita overflow.

## Validación previa

1. Existen exactamente 19 diapositivas.
2. Cada diapositiva contiene los 15 campos requeridos.
3. Cada afirmación tiene status y fuente.
4. Cada número tiene unidad, fecha y fuente.
5. No se presenta arquitectura propuesta como implementación productiva.
6. El estudiante aparece sólo como beachhead B2C provisional.
7. Se conservan AI Agents, Verified Human Progress, Pilot, Governance, NVIDIA, Roadmap, Founder y Ask.
8. El MVP y la arquitectura objetivo están separados.
9. Los placeholders no se convierten en hechos.
10. Los diagramas y gráficas quedan editables.
11. El deck responde qué hace la plataforma, para quién empieza, cómo funciona, cómo madura y qué evidencia falta.

## Entregables

- Especificación completa para 19 diapositivas.
- Texto visible y notas del presentador.
- Plan visual por diapositiva.
- Matriz de pendientes y claims por validar.
- PPTX editable.
- PDF exportado.
- Render de revisión visual con verificación de legibilidad, alineación, clipping y consistencia.

No generes el PPTX o PDF hasta que el contenido cumpla la validación anterior.

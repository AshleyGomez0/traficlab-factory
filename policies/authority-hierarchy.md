# Authority Hierarchy

## Highest to lowest

```
GitHub remote       = hechos, SHAs, PRs, branches, merges, issues
.hermes/control-plane/ = operación/ownership en tiempo real
PROJECT_STATE / WORKLOG / docs = estado documental de producto
Obsidian            = conocimiento, arquitectura, decisiones, investigación
Chat                = transporte temporal, NO autoridad durable
```

## Product ownership

```
HERMES-ORCH  → TRAFFICLABPRO_CONTROL
HERMES-ORCH  → panorama-mission-control  # Segundo Cerebro / Obsidian / Knowledge Loop (ID existente, no duplicar registro)
HERMES-IA    → IA-VISION
HERMES-SUINI → SUINI
```

## Cross-product rule

```
if target_product != assigned_product:
  STOP
  PRODUCT_OWNERSHIP_MISMATCH
  RETURN_TO_ORCHESTRATOR
```

## Cross-repository authority for Segundo Cerebro

El identificador estable existente para la organizacion de Obsidian/conocimiento es `panorama-mission-control` (`01_PROJECTS/PANORAMA/PROJECT.md` y `99_SYSTEM/project_registry/README.md`). No crear `PANORAMA_CONOCIMIENTO` ni un segundo proyecto de runtime.

El contrato de conocimiento y revision se mantiene por referencia, no se copia: [Mission Control Knowledge Loop](https://github.com/neokyhurtado-cmd/panorama-mission-control/blob/main/09_PROTOCOLS/KNOWLEDGE_LOOP_V1.md). Esta referencia no instala hooks, no convierte a Simon/Vera en cuentas, no modifica identidades ni concede permisos a los runtimes separados.

**Decision Ashley D2 (2026-11-17):** HERMES-ORCH tiene ruta funcional al producto `panorama-mission-control`/Segundo Cerebro. El acceso real a Git, Obsidian y la ejecucion sigue sujeto a identidad tecnica, permisos por recurso, contrato de escritor unico y QA. No extrapolar autoridad de un producto a otro.

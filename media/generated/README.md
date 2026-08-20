# GENERATED — AKAI

> Esta carpeta NO contiene imagenes. Es un puntero: las imagenes generadas reales viven en Jockey.

## Jockey Knowledge Store

```text
Nombre: AKAI — Generated
Store ID: ks_01a017b8-efe3-73b0-a1b7-d610700acbaf
```

## Contenido

Vacío por ahora. Esta store se puebla con salidas de Higgsfield conforme se generen, con metadata de estado:
- `pending` — salida inicial sin aprobacion humana.
- `changes_requested` — requiere correcciones (delta: KEEP / CHANGE / PROTECT).
- `approved` — aprobado por humano. Si se vuelve reusable, se promueve a FINAL_ASSETS.

Ver `context/IMAGE_APPROVAL_WORKFLOW.md` para el flujo de aprobación.

## Cómo usar (Claude Code / MCP)

1. Llamar `jockey_add_media` con `knowledge_store_id: ks_01a017b8-efe3-73b0-a1b7-d610700acbaf` al registrar una generación de Higgsfield, con metadata `collection: GENERATED` y `status: pending|changes_requested|approved`.
2. Llamar `jockey_list_knowledge_store_items` o `jockey_search` sobre el mismo store para consultar.
3. No descargar copias permanentes al repo — solo temporales si una integración lo requiere.

Ver también `media/JOCKEY_LIBRARY.md` y `media/MEDIA_INDEX.md`.

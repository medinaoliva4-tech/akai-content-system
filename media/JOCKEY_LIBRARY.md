# Jockey Media Library — AKAI

## Nota sobre subcarpetas

Jockey no soporta subcarpetas dentro de un mismo knowledge store. Por eso, siguiendo instrucción de Rodrigo, la biblioteca de AKAI se dividió en **tres knowledge stores separados** (uno por colección), en vez de una sola store con carpetas internas.

## AKAI — Originals

```text
Nombre: AKAI — Media Library (funciona como "Originals")
Store ID: ks_01a0177d-efe6-7363-b28d-c5c7ff668cf9
```

Estado: **182 items subidos** desde Google Drive (dos carpetas de fotografía de producto: "2025 (utiles para diseños 2026)" y "2026 (utiles para diseños 2026)"). Procesamiento en Jockey en curso (ready/queued/processing) al momento de la carga — 0 fallos. Cada item tiene metadata `collection: ORIGINALS` y `title` con el nombre de archivo original.

Fuentes Drive:
- https://drive.google.com/drive/folders/1wiZFhHUQmBo4zsqoAg9sjJBr8WSTqumT (172 fotos)
- https://drive.google.com/drive/folders/1CmuQVBxtAA7oTYA3MFfUULRNvOzlhWmJ (9 fotos)

## AKAI — References

```text
Store ID: ks_01a017b8-e6ee-72e2-bd8a-a19522725420
```

Estado: creado, vacío. Poblar cuando se clasifiquen referencias visuales (brand world, inspiración) desde `brand_world_reference/`.

## AKAI — Generated

```text
Store ID: ks_01a017b8-efe3-73b0-a1b7-d610700acbaf
```

Estado: creado, vacío. Poblar conforme se generen y aprueben piezas con Higgsfield (ver `context/IMAGE_APPROVAL_WORKFLOW.md`).

## Regla

Todas las imagenes y videos de la marca viven en Jockey.

GitHub no debe almacenar copias de produccion salvo que una integracion necesite temporalmente un archivo local para operar. Esos temporales no son fuente de verdad y deben quedar fuera de la biblioteca permanente.

Claude debe consultar Jockey antes de:
- buscar referencias;
- solicitar una nueva generacion;
- seleccionar fotografia para Figma;
- asumir que falta un asset.

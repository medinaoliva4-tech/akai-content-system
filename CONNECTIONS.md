# CONNECTIONS.md — Estado de integraciones y preflight

> Archivo variable por cliente/operador. La estructura del repo no basta: una integración crítica sin configurar puede bloquear producción. `OPERATIONS.md` define cómo conectar y verificar cada herramienta; aquí se registra el estado real.

## Regla

Estados permitidos:
- `READY`
- `NOT_CONFIGURED`
- `BLOCKED`
- `NOT_REQUIRED`

No marcar una conexión como `READY` solo porque exista un README. Debe haberse probado en el entorno que la va a usar.

## GitHub / repo
- Estado: NOT_CONFIGURED
- Repo remoto: POR DEFINIR
- Branch: main
- Lectura/clonado validado: POR DEFINIR
- Write-back disponible: POR DEFINIR
- Último commit remoto validado: POR DEFINIR

## Figma Desktop
- Estado: NOT_CONFIGURED
- Archivo/proyecto principal: POR DEFINIR
- Página/sistema base: POR DEFINIR
- Última prueba: POR DEFINIR

## Figwright MCP
- Estado: NOT_CONFIGURED
- Servidor MCP detectado por Claude Code: POR DEFINIR
- Plugin local conectado a Figma Desktop: POR DEFINIR
- Última prueba de lectura/escritura: POR DEFINIR

## Jockey MCP
- Estado: READY
- Endpoint: `${JOCKEY_MCP_URL:-https://mcp.twelvelabs.io/jockey/mcp}`
- OAuth validado: SÍ (conexión MCP activa)
- Knowledge stores de marca: AKAI — Originals (`ks_01a0177d-efe6-7363-b28d-c5c7ff668cf9`, 182 items), AKAI — References (`ks_01a017b8-e6ee-72e2-bd8a-a19522725420`, vacío), AKAI — Generated (`ks_01a017b8-efe3-73b0-a1b7-d610700acbaf`, vacío)
- Nota: Jockey no soporta subcarpetas dentro de una store; se usaron 3 stores separadas por colección.
- Link directo documentado en `media/JOCKEY_LIBRARY.md`: SÍ
- Busqueda de prueba ejecutada: POR DEFINIR
- Consulta de colecciones/metadata validada: SÍ (`jockey_list_knowledge_store_items` con readiness)
- Alta/registro de media aprobada validado: SÍ — 182 fotografías originales de producto subidas desde Google Drive el 2026-08-19, 0 fallos. References y Generated aún vacíos.

## Higgsfield Cinema Studio
- Estado: NOT_CONFIGURED
- Proyecto del cliente: POR DEFINIR
- Folder/categoría: POR DEFINIR
- Sesión accesible: POR DEFINIR
- Preset/cámara documentado: POR DEFINIR
- Última prueba de generación: POR DEFINIR

## Apify
- Estado: NOT_CONFIGURED
- Apify plugin/MCP habilitado en Claude Code: POR DEFINIR
- OAuth/token validado: POR DEFINIR
- Actor de prueba ejecutado: POR DEFINIR
- Dataset de prueba recuperado: POR DEFINIR
- Última prueba: POR DEFINIR

## Metadata2Go
- Estado: NOT_CONFIGURED
- Acceso web validado: POR DEFINIR
- Flujo `Remove Metadata` validado con export de prueba: POR DEFINIR
- Verificación posterior de metadatos: POR DEFINIR
- Última prueba: POR DEFINIR

## Publicación / distribución
- Herramienta: POR DEFINIR
- Estado: NOT_REQUIRED
- Última prueba: POR DEFINIR

## Bloqueos activos
POR DEFINIR

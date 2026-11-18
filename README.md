# Longevix QA · Vistas del tablero Scheduling

Página para ver y manejar las tarjetas del tablero de Trello "Longevix QA CU Scheduling" con vistas que Trello gratis no tiene: Tabla, Por estado, Por lista y Resumen.

Link: https://geronimo-bassi.github.io/longevix-qa-board/

## Cómo se usa

1. Abrí el link.
2. Tocá **Conectar Trello**. Se abre trello.com: tocá **Allow** y volvés a la página.
3. Listo. Ves las tarjetas con tu cuenta, y lo que cambies queda con tu nombre en Trello.

- El permiso dura 30 días y queda guardado solo en tu navegador. No pasa por ningún servidor nuestro: la página habla directo con Trello.
- Para cortarlo, tocá **Desconectar**, o en Trello: foto de perfil › Settings › Applications › Revoke.
- Tu usuario de Trello tiene que ser miembro del tablero.

## Qué se puede hacer

- Filtrar por tipo, prioridad, estado, quién la creó y lista; buscar texto.
- Abrir una tarjeta: descripción, comentarios y quién la creó.
- Cambiar estado (FIXED / Rechequear / Reportado) y etiquetas, mover de lista, archivar.
- Comentar con @menciones (autocompletado) y editar o borrar tus comentarios.
- **➕ Nueva tarjeta** con la plantilla de la casa y aviso de posibles duplicados.
- Todo cambio pide confirmación antes de escribir en Trello.

## Para quien mantiene la página

- Todo está en `index.html`. La API key de Trello va en `const TRELLO_KEY = "..."`. La API key es pública por diseño; el **Secret** nunca va acá.
- En la configuración de la key (trello.com/power-ups/admin), "Allowed origins" tiene que incluir `https://geronimo-bassi.github.io`.
- Para publicar un cambio: commit y push a `main`; GitHub Pages lo actualiza en 1–2 minutos.

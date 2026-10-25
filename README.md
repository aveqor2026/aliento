# Aliento · Afirmaciones

App de respiración (Ronda / Calma / Caja) con **una afirmación en la pausa**. Para Ismael.

## Abrir en el teléfono

URL pública (GitHub Pages):

**https://aveqor2026.github.io/aliento/**

Agrégala a la pantalla de inicio del teléfono (Compartir → Añadir a inicio).

## Editar las 9 afirmaciones

1. Abre la app → toca **Afirmaciones** (arriba a la derecha).
2. Cambia las frases → **Guardar**.
3. Quedan en este teléfono (`localStorage`). La rotación empieza de nuevo con esa lista.
4. **Volver a las 9 de inicio** restaura las frases originales.

## Rotación

En cada pausa (hold) aparece **una** frase. No se repite hasta agotar las 9. Si paras a la 2, la siguiente sesión sigue con las que faltan.

## Desarrollo local

```bash
cd /workspace/aliento-afirmaciones
python3 -m http.server 8765
# http://localhost:8765
```

Archivos: `index.html`, `app.js`, `afirmaciones.js`, `s.css`, `extra.css`.

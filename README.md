# Aliento · Afirmaciones + sync hábitos

App de respiración (Ronda / Calma / Caja) con afirmación en la pausa y **envio automático al registro de hábitos** al terminar la sesión.

## Abrir

**https://aveqor2026.github.io/aliento/**

## Contéo → hábitos

Al terminar una sesión con al menos 1 ronda/ciclo:

| En la app | En el CSV |
|-----------|-----------|
| 1 hold / ciclo completado | +1 `respiraciones` |
| 3 holds en una sesión | fila con `cantidad=3` |

Fecha = día en America/New_York.

## Conectar sync (una vez por dispositivo)

1. El bot crea la routine webhook «Aliento → hábitos» (ver `PARENT_ROUTINE.md`).
2. En desktop, abre la routine y copia **POST to** + **key**.
3. En la app: **Afirmaciones** → sección **Hábitos (sync)** → pega URL y key → **Guardar sync** → **Probar sync**.
4. Haz lo mismo en el iPad.

La key solo vive en el teléfono/iPad (`localStorage`). No está en este repo.

## Afirmaciones

Edítalas en **Afirmaciones**. Rotan sin repetir hasta agotar la lista.

## Desarrollo

```bash
cd /workspace/aliento-afirmaciones
python3 -m http.server 8765
```

Archivos clave: `app.js`, `afirmaciones.js`, `sync.js`.

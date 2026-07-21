# Torneo de fútbol · WebApp responsive

Aplicación mobile-first autocontenida para simular la última jornada, recalcular clasificaciones y mostrar los cruces de semifinales.

## Cómo abrirla

1. Descarga la carpeta o el ZIP.
2. Abre `index.html` en un navegador moderno.
3. Se necesita conexión a Internet únicamente para cargar Tailwind CSS desde su CDN.

También puedes servirla localmente:

```bash
python -m http.server 8080
```

Después abre `http://localhost:8080`.

## Funciones

- Marcadores táctiles con botones `+` y `-`.
- Clasificación en tiempo real.
- Desempates por enfrentamiento directo, minitorneo, diferencia de goles, goles a favor y edad acumulada.
- Semifinales dinámicas.
- Calendario, resultados y sanciones.
- Diseño mobile-first con navegación inferior fija.

## Nota sobre los resultados históricos

El JSON contiene una clasificación tras dos jornadas, pero solo incluye un partido finalizado por equipo. Para aplicar correctamente el enfrentamiento directo, la aplicación reconstruye los cuatro resultados que faltan restando los marcadores visibles a las estadísticas acumuladas. La reconstrucción es única y coherente con GF/GC y puntos.

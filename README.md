# TopoCrime

Prototipo interactivo para explorar hotspots de delito sobre la red vial de
Lima Metropolitana (2018–2025) y comparar zonas con la misma forma de calles.

**Demo:** https://cesarpr30.github.io/TopoCrime/

Funciona en laptop, iPad y celular. En celulares (pantalla táctil angosta)
arranca en un solo mes, con la línea de tiempo plegada, limita el periodo a 6
meses y carga las POIs solo al activarlas: así la memoria cabe en Safari de
iPhone. `?modo=completo` abre la versión completa.

## Qué muestra

- **Mapa:** 1 016 306 denuncias de la PNP en la vía pública, como puntos, por
  nodo de la red, como mapa de calor o en relieve 3D.
- **Subgrafos:** 4 299 hotspots significativos (test Monte Carlo) extraídos
  sobre la red vial.
- **Ficha del subgrafo:** delitos, nodos, tipos de delito y POIs de la zona.
- **Gemelos:** zonas con la misma estructura de calles (huella de forma sin
  crimen) y su comparación A vs B.

## Contenido

```
index.html                  dashboard
como-funciona*.html         explicación del método
data/lima/                  artefactos del pipeline, versión ligera
```

Los datos son una versión reducida de los del pipeline: geometrías
simplificadas (≈1 m) y solo el embedding principal (graph2vec).

Autores: César Pajuelo, Germain García · Universidad de Ingeniería y
Tecnología (UTEC).

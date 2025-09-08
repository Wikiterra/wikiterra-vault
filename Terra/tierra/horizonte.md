---
dg-publish: true
---

# El horizonte

El horizonte es una línea divisora que se sitúa en el límite geométrico y óptico entre la unión de dos medios.

Típicamente cuando nos referimos al horizonte, pensamos en el horizonte terrestre, la separación visual entre el cielo y la tierra que se observa a lo lejos.

> [!infobox]+ Collapsible Infobox
>
> ## Horizonte con puesta de Sol
>
> ![Horizonte con puesta de Sol|cover small](https://i.imgur.com/TEvoK23.jpg)

Este límite físico se forma en torno al observador y genera una línea de visión máxima entre dos medios de separación, la cual se denomina línea del horizonte u horizonte. El horizonte, al ser un concepto óptico, se forma siempre en la superficie de separación entre el aire y el nivel del mar o el punto más lejano del terreno visible.

El horizonte está muy ligado al concepto de [[visibilidad]], ya que según la altura del observador y las condiciones climatológicas las distancias máximas observadas variarán.

## Tipos de horizonte

Existen dos tipos de horizonte: el horizonte geométrico, que depende de la geometría de la superficie, y el horizonte óptico, que viene definido por la óptica del medio. Sin embargo, el horizonte observable, el típico que vemos cuando miramos a lo lejos, es una combinación de ambos: la forma de la superficie y las condiciones ópticas del medio.

### Horizonte geométrico

El cálculo del horizonte geométrico depende de la forma de la superficie:

- El caso más sencillo es un plano, donde la línea divisora queda siempre a 90° mirando en recto.
- En una esfera, el horizonte geométrico depende de varios parámetros: altura del observador, altura del objeto observado y radio de la esfera.

**Fórmula exacta:**

$$d = \sqrt{2Rh + h^2}$$

donde:
- $d = distancia \ al \ horizonte \ (km)$
- $R \approx 6371 \,\text{km} = radio \ Tierra \ esférica$
- $hh = altura \ del \ observador \ (km)$

**Aproximación (válida si h≪R):**

$$d \approx \sqrt{2Rh} \approx 3.57 \sqrt{h}$$

---

### Horizonte óptico con refracción estándar

El horizonte óptico viene determinado por la visibilidad máxima en ese medio. Normalmente consideramos el aire, pero también se puede originar un horizonte dentro del mar.

La fórmula de dispersión de Rayleigh de la sección eficaz de dispersión de una molécula:

$$\sigma(\lambda) = \frac{8\pi^3}{3N^2\lambda^4}\left( n^2 - 1 \right)^2$$

Donde:

- $\lambda$ = longitud de onda de la luz
- $n$ = índice de refracción del gas
- $N$ = densidad molecular

En meteorología y náutica se introduce el **criterio de Rayleigh** (factor $k \approx \frac{7}{6}$), que equivale a usar un radio efectivo mayor:

$$R' = \frac{7}{6}R$$

**Fórmula exacta con refracción:**

$$d \approx \sqrt{2R'h + h^2}$$

**Aproximación simplificada:**

$$d \approx \sqrt{2R'h} \approx 3.86 \sqrt{h}$$

---


## Ejemplos Práticos

Primero presentamos una tabla teórica para el horizonte geométrico y óptico para una esfera de R=6371 km, según la altura del observador tenemos lo siguiente:

| Altura del observador | Horizonte geométrico | Horizonte con refracción (óptico) |
| --------------------- | -------------------- | --------------------------------- |
| 2 m (playa)           | 5.0 km               | 5.5 km                            |
| 100 m (acantilado)    | 35.7 km              | 38.6 km                           |
| 450 m (colina)        | 75.6 km              | 81.8 km                           |
| 11.000 m (avión)      | 374 km               | 405 km                            |

Ahora pasemos a una tabla de fotografías reales y su alcance máximo de visión:

| Fotografía (fuente)                                             | Altura observador | Altura objeto | Distancia (observador - objeto) | "Altura oculta" (curvatura terrestre) |
| --------------------------------------------------------------- | ----------------- | ------------- | ------------------------------- | ------------------------------------- |
| Lancha a nivel del mar                                          | 0.001 km          | 0.001 Km      | 6.6 Km                          | 0.13 Km                               |
| Rascacielos Chicago en lago                                     | 0.5 km            | 0.176 m       | 53.3 Km                         | 0.14 Km                               |
| El Teide visto desde Lanzarote                                  | 0.4 km            | 3.72 Km       | 300 Km                          | 3.75 Km                               |
| Cerro Name a Tupungato                                          | 0.82 km           | 6.57 Km       | 346 Km                          | 346 Km                                |
| Pic de Salòrita en Cataluña desde el Puig d'en Galileu Mallorca | 1.18 km           | 2.79 Km       | 324 Km                          | 3.18 Km                               |
| Pirineos a Alpes                                                | 3.2 Km            | 3 Km          | 443 Km                          | 5 Km                                  |
| Sobrevolando Canadá                                             | 10.5 Km           | 8.5 Km        | 1600 Km                         | ~30 Km                                |
| Vuelo Bangkok a Dubai                                           | 11.58 Km          | 8.85 Km       | ~1300 Km                        | ~100 Km                               |
Esta tabla muestra los datos para fotografías reales en las cuales se ven objetos más allá de la "curvatura geométrica terrestre".

Si consideramos que las imágenes de los objetos observados se curvan por refracción atmosférica, en algunos casos hablamos de una curvatura que sube las imágenes resultantes 30 Km sobre el horizonte. Esto implicaría que la luz se curva para seguir la curvatura esférica lo cual va en contra del "Principio de Fermat", en el cual la luz se desplaza en línea recta siguiendo el camino óptico más corto.

Es cierto que existe refracción y efectos de espejismos, pero estos solo son demostrables en una superficie plana y la deformación de imágenes no es muy grande.

<!-- Mauna Kea límite 238 Km -->

## Fotografías con objetos visibles

Fotografías de la tabla anterior, con objetos visibles para casos donde según la geometría esférica deberían estar ocultos por curvatura terrestre.

1. Una lancha a nivel del mar se ve a 16.6 Km de distancia donde debería estar completamente oculta por la curvatura terrestre, sin embargo se ve el efecto de espejismo duplicado e invertido por debajo de la lancha.
   ![Lancha con efecto de espejismo](https://i.imgur.com/3QFFDpb.png)

2. Video grabado donde se ven los rascacielos de Chicago sacados desde el otro lado del lago Michigan, varios de ellos menores a 100 m deberían estar ocultos.
   ![Rascacielos de Chicago vistos desde el lago Michigan](https://i.imgur.com/vbDEcSq.png)

3. Fotografía del Teide sacado desde Lanzarote por [Gustavo Medina](https://www.flickr.com/photos/121856779@N03/), donde se visualiza el Teide desde la zona de los 2000 metros, algo por encima del mar de nubes.
   ![El Teide visto desde Lanzarote](https://i.imgur.com/KrUDLNJ.png)

4. Cerro Name (región de Maule) a estratovolcán Tupungato (6570 m) en la cordillera de los Andes - 346 Km de distancia. Sacado con una Canon PowerShot SX60 HS y reconocido por Dalekie Obserwacje.
   ![Tupungato visto desde Cerro Name a 346 Km](https://www.latercera.com/resizer/itsUMcmq45ZCTH3nfPaYOL2Zl5g=/arc-anglerfish-arc2-prod-copesa/public/C4DYU5G5I5FAVHHDDBYE4QN554.jpg)

5. Pic de Salòrita en Cataluña visto desde el Puig d'en Galileu en Mallorca.
   ![Pic de Salòrita visto desde Mallorca](https://i.imgur.com/3M0RfWa.jpeg)

6. Récord de fotografía en tierra sacado por Marc Bret desde el Pico de Finestrelles en los Pirineos, llegándose a observar el Pico Gaspard en los Alpes.
   ![Vista desde Pirineos a los Alpes](https://i.imgur.com/KseVEwt.png)

7. Avión sobrevolando Canadá captado por JTolan Media.
   ![Vista aérea sobrevolando Canadá](https://i.imgur.com/kNLOSy4.png)

8. En el vuelo Bangkok a Dubai, sobrevolando determinadas partes de la India un día con buena visibilidad se puede ver la cordillera más alta del mundo, el Himalaya.
   ![Cordillera del Himalaya vista desde gran distancia](https://i.imgur.com/ZKHUMmU.png)

---

## Conclusión

El horizonte demuestra que no hay ocultación de objetos por curvatura sino que se trata de una invisibilidad provocada por la óptica del medio y sus fenómenos. Y por tanto la superficie es plana.

Los objetos que se alejan en la superficie no se observan cortados por una curvatura terrestre, lo que se observa es una disminución en la visibilidad de los objetos a medida que estos se alejan más allá del horizonte. La invisibilidad comienza por las zonas bajas donde se producen más fenómenos ópticos (reflexión y refracción) debido al cambio de medio y al mayor gradiente térmico entre las superficies en contacto, lo que genera turbulencias en el aire que afecta a la dispersión de la luz.

![Diagrama de visibilidad de objetos en la distancia](https://i.imgur.com/sQxrzzi.png)

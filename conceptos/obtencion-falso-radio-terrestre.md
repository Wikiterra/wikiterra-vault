---
dg-publish: false
---

# Obtención del falso radio terrestre a partir de la resolución óptica

Esta imagen muestra como se extrajo el falso "radio terrestre" del modelo Tierra esférica a partir de la **resolución angular del ojo humano**, pasando de un horizonte óptico a un falso horizonte geométrico.

![](https://i.imgur.com/YTfaFR0.png)

---

## 🔍 Paso a paso del razonamiento en la imagen:

### 1. **Resolución angular óptica**

Esta fórmula es una adaptación del **límite de difracción de Rayleigh**, usada para calcular la **resolución angular mínima (θ)** que puede lograr un sistema óptico:

$$\theta = 1.22 \cdot \frac{\lambda}{D}$$

donde:
- $\theta$: resolución angular en radianes
* $λ = 679.456 nm = 679.456  \cdot 10^{-9}$ (longitud de onda de la luz, casi rojo)
* $D = 2.21 mm = 2.21 \cdot 10 ^{-3}$ (diámetro de la pupila del ojo)

$$\theta = 1.22 \frac{679.456 \cdot 10^{-9}}{2.21 \cdot 10^{-3}} \approx 3.75 \cdot 10^{-4} \ \text{rad}$$
$$\theta_\text{deg} = 3.75\cdot10^{-4} \cdot \frac{180}{\pi} \approx 0.0215^\circ = 21.5 \text{ miligrados}$$

✅ Esto es una estimación razonable para el límite de resolución del ojo humano en condiciones ideales (aunque en la práctica, por aberraciones ópticas y del sistema nervioso, suele ser peor).

---

### 2. **Distancia al horizonte visual**

$$D = \frac{h}{tan(θ)}$$

donde:
$D$: distancia al horizonte
$h$: altura del observador en metros
$\theta$: resolución angular

Para una persona media de 1.80 metros de altura su límite visual es:
$$D = \frac{1.8}{3.75 \cdot 10^{-4}} \approx 4800 m \approx 4.8 \ km$$

---
### 3. **Cálculo del radio de esfera terrestre, considerando una ocultación debido a un horizonte geométrico**

#### Método 1: geometría esférica

Para un observador de altura **h** sobre una esfera de radio **R**, la distancia al horizonte **d** viene dada por el triángulo rectángulo formado por el centro de la esfera, el ojo y el horizonte:

$$d = \sqrt{2 R h + h^2} \approx \sqrt{2 R h} \Rightarrow R = \frac{d^2}{2 h} \quad (\text{ya que } d \ll R \text{ y } h \ll R)$$
donde:
$d$: distancia
$R$: radio de una esfera convexa
$h$: altura del observador

Ejemplo numérico, para $d = 4799\ \text{m}$ y $h = 1.8\ \text{m}$.
$$R \approx \frac{(4799)^2}{2 \cdot 1.8} \approx 6.4 \cdot 10^6 \ \text{m} \approx 6400 \ km$$


#### Método 2: aproximación usando resolución angular del ojo

Si consideramos la **resolución angular mínima** $\theta$ del ojo, el horizonte se “oculta” bajo un ángulo $2\theta$. Una aproximación lineal para ángulos muy pequeños da:

$$t$$

**Ejemplo numérico**, para $d = 4799 \ m$ y $2\theta = 00075 \ rad$.
$$R = \frac{d}{tan(2 \theta)} \Rightarrow R= \frac{4799}{tan(0.00075)} = 6399 km$$

> Esta fórmula **no proviene de la geometría esférica exacta**, sino de un razonamiento óptico basado en el límite de resolución angular del ojo. Funciona bien porque θ\thetaθ es muy pequeño $(tan(2\theta) \approx 2\theta)$.


## Conclusión

Esta breve explicación de fórmulas, pone de manifiesto que el horizonte geométrico y la derivación del radio para una esfera convexa, se pueden derivar del horizonte óptico. Y justamente en el caso de la superficie terrestre coincide que esa extracción un supuesto radio es de alrededor de 6400 km.

Esto significa que a partir de la óptica del globo ocular medio de una persona, se puede derivar el cálculo de una supuesta esfera terrestre de 6400 km de radio. Y esto implica que el modelo esférico justo se creo con esos datos para que visualmente desde la superfice con el ojo humano fuese indistinguible la ocultación por óptica que la ocultación por una curvatura esférica.

Sin embargo si usamos cámaras con lentes de largo alcance la cosa cambia, y se pueden observar distancias mucho más allá de ese falso horizonte geométrico.

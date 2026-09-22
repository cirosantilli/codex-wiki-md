<h1 id="3a/solution">Solution</h1>

↑ **Parent:** [3A](../3a.md)

Take upward as positive and let $dm<0$ be the change in rocket [mass](../../../../../mass.md) during $dt$. The exhaust emitted has mass $-dm$ and, to first order, upward velocity $v-U$. The [linear momentum](../../../../../momentum.md) of the rocket and just-emitted gas changes by

$$
(m+dm)(v+dv)+(-dm)(v-U)-mv=m\,dv+U\,dm+O(dt^2).
$$

The external gravitational impulse is $-mg\,dt$ to first order. Applying the momentum balance to this material system, rather than applying a fixed-mass formula to the rocket alone, gives the [rocket equation](../../../../../rocket-equation.md)

$$
\boxed{m\frac{dv}{dt}+U\frac{dm}{dt}=-mg.}
$$

The term $-U\dot m$ is the upward thrust.

For the specified mass loss and exhaust law, $\dot m=-\alpha$ and

$$
\dot v=\frac{\alpha U_0m_0}{(m_0-\alpha t)^2}-g,\qquad \dot v(0)=\frac{\alpha U_0}{m_0}-g.
$$

Thus the condition for strictly positive upward [acceleration](../../../../../acceleration.md) at launch is

$$
\boxed{\alpha U_0>m_0g.}
$$

At equality the initial thrust just balances the weight; under this particular exhaust law the acceleration becomes positive immediately afterwards. If the initial thrust is smaller than the weight and the rocket initially rests on a launch surface, a nonzero supporting force persists until a later lift-off, so the free-flight equation does not describe its earlier supported motion.

For immediate free flight, integrate the [rocket equation](../../../../../rocket-equation.md) with $v(0)=0$:

$$
v(t)=U_0m_0\left(\frac1{m_0-\alpha t}-\frac1{m_0}\right)-gt,\qquad \boxed{v(t)=\frac{U_0\alpha t}{m_0-\alpha t}-gt}.
$$

This applies while $0\leq t<m_0/\alpha$ and the nonrelativistic approximation remains valid. The formal divergence as the model's remaining mass approaches zero is not a prediction within that approximation.

For [dimensional analysis](../../../../../dimensional-analysis.md), write the mass, length and time dimensions as $\mathsf M,\mathsf L,\mathsf T$. Then $[m_0]=[m]=\mathsf M$, $[\alpha]=\mathsf M\mathsf T^{-1}$, $[t]=\mathsf T$, $[U_0]=[U]=[v]=\mathsf L\mathsf T^{-1}$, and $[g]=\mathsf L\mathsf T^{-2}$. Both $m_0$ and $\alpha t$ have mass dimension, so $\alpha t/(m_0-\alpha t)$ is dimensionless; both terms in the boxed velocity have dimension $\mathsf L\mathsf T^{-1}$. The launch inequality compares two forces, each of dimension $\mathsf M\mathsf L\mathsf T^{-2}$.

## ↑ Ancestors (10)

1. [3A](../3a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

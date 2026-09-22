<h1 id="13d/solution">Solution</h1>

↑ **Parent:** [13D](../13d.md)

In [polar coordinates](../../../../../polar-coordinates.md),

$$
v\,dt=ds=\sqrt{dr^2+r^2d\theta^2}.
$$

With the change of radial coordinate $u=\log r$, the detection functional becomes

$$
P=\lambda\int\frac{ds}{r}
=\lambda\int\sqrt{du^2+d\theta^2}.
$$

It is therefore $\lambda$ times ordinary [path length](../../../../../arc-length.md) in the $(u,\theta)$-plane. The shortest path is the line segment from $(\log A,0)$ to $(\log B,\alpha)$, so

$$
u(\theta)=\log A+\frac{\log(B/A)}{\alpha}\theta.
$$

Returning to $r$ gives the [logarithmic spiral](../../../../../logarithmic-spiral.md)

$$
\boxed{r(\theta)=A\exp\!\left(\frac{\log(B/A)}{\alpha}\theta\right)}.
$$

Its minimum detection probability is

$$
P_{\min}=\lambda\sqrt{\log^2(B/A)+\alpha^2}.
$$

The functional depends only on the geometric path and not its parametrization, so tiptoeing and running give the same probability.

For the improved sensor, omit the irrelevant positive factor $\lambda$ and use the [Lagrangian](../../../../../lagrangian.md)

$$
L=\frac{\dot r^2}{r}+r\dot\theta^2.
$$

The coordinate $\theta$ is cyclic, so its [conjugate momentum](../../../../../canonical-momentum.md) is conserved. Equivalently,

$$
\boxed{h=r\dot\theta}
$$

is constant. Because $L$ has no explicit time dependence, the associated [conservation of energy](../../../../../conservation-of-energy.md) gives the constant

$$
\boxed{E=\frac{\dot r^2}{r}+r\dot\theta^2}.
$$

Multiplying by $r$ and using $h=r\dot\theta$ gives the required equation

$$
\boxed{\dot r^2=Er-h^2}.
$$

## ↑ Ancestors (10)

1. [13D](../13d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

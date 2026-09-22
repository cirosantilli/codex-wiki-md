<h1 id="s01/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the small clockwise [contour](../../../../../complex-integration-contour.md) $z=\epsilon e^{i\theta}$, $\theta$ decreases from $\pi$ to $-\pi$. Uniformly on that arc, $e^{z-\sqrt z}=1+O(\sqrt\epsilon)$, and hence

$$
\int_{C_4}F(z)\,dz=i\int_\pi^{-\pi}\bigl(1+O(\sqrt\epsilon)\bigr)\,d\theta\longrightarrow-2\pi i.
$$

The large arcs also vanish. To make this precise for the displayed geometry, take them on the left semicircle $z=\gamma+Re^{i\theta}$, $\pi/2\le\theta\le3\pi/2$, split at the cut. On the principal [holomorphic branch](../../../../../holomorphic-branch.md), $\operatorname{Re}\sqrt z\ge0$, $|z|\ge R-\gamma$, and $\operatorname{Re}z=\gamma+R\cos\theta$. The [estimation lemma](../../../../../estimation-lemma.md) gives

$$
\left|\int_{C_2\cup C_6}F\,dz\right|\le\frac{Re^\gamma}{R-\gamma}\int_{\pi/2}^{3\pi/2}e^{R\cos\theta}\,d\theta=O(R^{-1}).
$$

For the last bound, symmetry and $\sin u\ge2u/\pi$ on $0\le u\le\pi/2$ imply that the angular integral is at most $\pi/R$. The exact choice of large arcs does not affect the limiting result. The vertical [improper integral](../../../../../improper-integral.md) converges absolutely because $e^{-\operatorname{Re}\sqrt{\gamma+iy}}/|\gamma+iy|$ decays as $O(e^{-c\sqrt{|y|}}/|y|)$.

Taking limits in the closed [contour integral](../../../../../contour-integral.md) now yields $2\pi iJ+2iK-2\pi i=0$, where $K=\int_0^\infty e^{-x}\sin(\sqrt x)\,dx/x$. Thus

$$
\boxed{J=1-\frac1\pi\int_0^\infty e^{-x}\frac{\sin\sqrt x}{x}\,dx.}
$$

As an optional explicit evaluation, put $x=t^2$ and define $K(a)=2\int_0^\infty e^{-t^2}\sin(at)\,dt/t$. [Differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) and the [Gaussian integral](../../../../../gaussian-integral.md) give $K'(a)=\sqrt\pi e^{-a^2/4}$ and $K(0)=0$. Therefore $K=K(1)=\pi\operatorname{erf}(1/2)$ and $J=\operatorname{erfc}(1/2)\simeq0.479500$ in terms of the [error function](../../../../../error-function.md) and [complementary error function](../../../../../complementary-error-function.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [S01](../../../s01.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

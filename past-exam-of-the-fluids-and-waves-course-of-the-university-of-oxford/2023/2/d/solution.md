<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the prescribed orientation $\alpha$ and strength $m$ fixed, and now let the doublet position $b(t)$ be complex. The [Milne-Thomson circle theorem](../../../../milne-thomson-circle-theorem.md) applies instantaneously with

$$
W(z,t)=\frac{M}{z-b}+\frac{\bar M z}{a^2-\bar b z},\qquad M=me^{i\alpha}.
$$

When taking its spatial derivative, $b(t)$ is a parameter. Removing the doublet's own singular term leaves the regular [complex velocity](../../../../complex-velocity.md) at its position:

$$
q_{\rm reg}(b)
=\left.\frac{\bar M a^2}{(a^2-\bar b z)^2}\right|_{z=b}
=\frac{\bar M a^2}{(|b|^2-a^2)^2}.
$$

Because $q=u-iv$, the stipulated [image-induced motion of a planar doublet](../../../../image-induced-motion-of-a-planar-doublet.md) obeys $\dot b=\overline{q_{\rm reg}(b)}$, not $q_{\rm reg}(b)$ itself. Hence

$$
\boxed{\dot b=\frac{ma^2e^{i\alpha}}{(|b|^2-a^2)^2}}.
$$

Its direction is constant. Indeed $\operatorname{Im}(be^{-i\alpha})$ is constant and, since $b(0)=b_0>a$ is real, equals $-b_0\sin\alpha$. Writing $b=re^{i\theta}$ in [polar coordinates](../../../../polar-coordinates.md) gives the path equation

$$
\boxed{r\sin(\theta-\alpha)=-b_0\sin\alpha},
\qquad
\boxed{r(\theta)=\frac{b_0\sin\alpha}{\sin(\alpha-\theta)}}
$$

where the quotient is used when $\sin\alpha\ne0$ and the branch through $(r,\theta)=(b_0,0)$ with $r>a$ is selected. It is the straight line through $b_0$ parallel to $e^{i\alpha}$. An unambiguous parametrization, also covering the degenerate polar cases, is

$$
b=b_0+s e^{i\alpha},\qquad
\dot s=\frac{ma^2}{(|b_0+s e^{i\alpha}|^2-a^2)^2},\qquad s(0)=0.
$$

If $\sin\alpha=0$, the path is radial along the positive real axis, with $\theta=0$ and changing $r$; it cannot be represented as a single-valued $r(\theta)$. The sign of $m$ selects which direction along the line is followed. These paths apply only while the singularity remains outside the obstacle; the model prescribes no orientation evolution.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

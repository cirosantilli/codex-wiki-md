<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $T$ for transit time and $\ell(y)=t_0-\alpha y^2$ for lens thickness to avoid using $t$ for both. In the [thin lens](../../../../thin-lens.md) approximation, the two geometrical distances to the lens plane are $\sqrt{a^2+d^2}$ and $\sqrt{b^2+d^2}$. Their sum counts the lens segment as vacuum. Replacing that segment by material of [refractive index](../../../../refractive-index.md) $n$ adds $(n-1)\ell(d)$ to the [optical path length](../../../../optical-path-length.md). Thus, to the retained thin-element accuracy,

$$
cT=\sqrt{a^2+d^2}+\sqrt{b^2+d^2}+(n-1)(t_0-\alpha d^2).
$$

Using the [Taylor expansion](../../../../taylor-expansion.md) $\sqrt{1+u}=1+u/2+O(u^2)$ for $d\ll a,b$ gives

$$
\boxed{T=\frac1c\left[a\left(1+\frac{d^2}{2a^2}\right)+b\left(1+\frac{d^2}{2b^2}\right)+(n-1)(t_0-\alpha d^2)\right].}
$$

The omitted geometrical terms include $O(d^4/a^3+d^4/b^3)$ in [optical path length](../../../../optical-path-length.md), together with finite-thickness corrections discarded by the [thin lens](../../../../thin-lens.md) and [paraxial approximations](../../../../paraxial-approximation.md). The addition is $n-1$, because the underlying distance already includes propagation across the thickness once in vacuum.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [11](../../11.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

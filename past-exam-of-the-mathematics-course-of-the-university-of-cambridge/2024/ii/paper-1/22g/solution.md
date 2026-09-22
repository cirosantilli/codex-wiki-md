<h1 id="22g/solution">Solution</h1>

↑ **Parent:** [22G](../22g.md)

The [closest point theorem in a Hilbert space](../../../../../hilbert-projection-theorem.md) states that every nonempty closed convex subset $C$ of a Hilbert space has a unique point nearest to any given $x$.

Let $d=\inf_{y\in C}\|x-y\|$ and choose $y_n\in C$ with $\|x-y_n\|\to d$. The parallelogram identity and convexity give

$$
\|y_n-y_m\|^2
=2\|x-y_n\|^2+2\|x-y_m\|^2
 -4\left\|x-\frac{y_n+y_m}{2}\right\|^2
\leq2\|x-y_n\|^2+2\|x-y_m\|^2-4d^2,
$$

so $(y_n)$ is Cauchy. Completeness and closedness give a [limit](../../../../../limit-of-a-function.md) $y\in C$ with $\|x-y\|=d$. If $y,z$ were both minimizers, the same identity with their midpoint would force $\|y-z\|=0$.

Apply the theorem to a closed subspace $F$. For $x\in H$, let $y\in F$ be closest and put $z=x-y$. For every $u\in F$, minimality of $\|z-tu\|^2$ at $t=0$ for real and imaginary $t$ gives $\langle z,u\rangle=0$. Hence

$$
x=y+z\in F+F^\perp.
$$

The intersection is zero, so $H=F\oplus F^\perp$.

If $T$ is a shift with orthonormal [basis](../../../../../basis.md) $(e_n)$, it is an isometry,

$$
(\operatorname{Im}T)^\perp=\operatorname{span}\{e_1\},
\qquad
\bigcap_{n\geq1}\operatorname{Im}(T^n)=\{0\}.
$$

Conversely, suppose these three properties hold. Choose a unit [vector](../../../../../vector.md) $e_1$ spanning $(\operatorname{Im}T)^\perp$ and set $e_n=T^{n-1}e_1$. Isometry makes this [sequence](../../../../../sequence.md) orthonormal. Iterating the orthogonal decomposition

$$
H=\operatorname{span}\{e_1\}\oplus\operatorname{Im}T
$$

gives

$$
H=\operatorname{span}\{e_1,\ldots,e_n\}\oplus\operatorname{Im}(T^n).
$$

A [vector](../../../../../vector.md) orthogonal to every $e_n$ lies in every $\operatorname{Im}(T^n)$ and is therefore zero. Thus $(e_n)$ is an orthonormal [basis](../../../../../basis.md) and $Te_n=e_{n+1}$, so $T$ is a shift. This is the [wandering-vector characterization of a unilateral shift](../../../../../wandering-vector-characterization-of-a-unilateral-shift.md).

## ↑ Ancestors (10)

1. [22G](../22g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

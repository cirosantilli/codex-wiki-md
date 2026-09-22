<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

We prove the [Casorati-Weierstrass theorem](../../../../casorati-weierstrass-theorem.md) by contradiction. Fix an allowed $\rho$. If the stated image were not a [dense set](../../../../dense-set.md) in $\mathbb C$, there would be a disc $B(w,\epsilon)$ disjoint from it. Hence

$$
|f(z)-w|\geq\epsilon\qquad(0<|z-a|<\rho).
$$

The [holomorphic function](../../../../holomorphic-function-split.md) $h(z)=1/(f(z)-w)$ is bounded by $1/\epsilon$ on that punctured disc. By the permitted [Riemann removable singularity theorem](../../../../riemann-removable-singularity-theorem.md), it extends to a [holomorphic function](../../../../holomorphic-function-split.md) $H$ on the full disc.

If $H(a)\ne0$, then $w+1/H$ is [holomorphic](../../../../holomorphic-function-split.md) near $a$ and agrees with $f$ away from $a$. This makes $a$ a [removable singularity](../../../../removable-singularity.md) of $f$.

If $H(a)=0$, then $H$ is not identically zero, since $h$ is nowhere zero away from $a$. Its [Taylor series](../../../../taylor-series.md) therefore has a finite first nonzero coefficient: otherwise the [identity theorem](../../../../identity-theorem.md) would make it identically zero. Write $H(z)=(z-a)^m K(z)$ with $m\geq1$ and $K(a)\ne0$. Then

$$
f(z)=w+\frac{(z-a)^{-m}}{K(z)}
$$

has a [pole](../../../../pole.md) of order $m$ at $a$, since multiplying by $(z-a)^m$ gives the nonzero limit $1/K(a)$.

Both cases contradict an [essential singularity](../../../../essential-singularity.md). Thus

$$
\boxed{\overline{f(B(a,\rho)\setminus\{a\})}=\mathbb C\quad\text{for every allowed }\rho>0}.
$$

## ↑ Ancestors (12)

1. [b](../b.md)
2. [4](../../4.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

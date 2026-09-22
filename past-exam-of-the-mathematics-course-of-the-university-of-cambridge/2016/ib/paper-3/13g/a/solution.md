<h1 id="13g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T$ be a closed triangle contained, together with a neighbourhood, in the domain of a [holomorphic function](../../../../../../holomorphic-function.md) $f$. We prove [Cauchy theorem for a triangle](../../../../../../cauchy-theorem-for-a-triangle.md) without assuming continuity of $f'$.

Join the edge midpoints to subdivide $T$ into four triangles, each with half its diameter and perimeter. Their positively oriented [contour integrals](../../../../../../contour-integral.md) sum to the integral around $T$, because the internal edges cancel. At least one subtriangle has integral of modulus at least one quarter of the original. Repeat that choice to obtain nested closed triangles $T_n$ satisfying

$$
\left|\int_{\partial T}f(z)\,dz\right|\leq4^n\left|\int_{\partial T_n}f(z)\,dz\right|,
\quad d_n=2^{-n}d_0,\quad P_n=2^{-n}P_0.
$$

Their intersection is a single point $z_*$, by compactness and shrinking diameter. [complex differentiability at a point](../../../../../../complex-differentiability-at-a-point.md) at $z_*$ gives

$$
f(z)=f(z_*)+f'(z_*)(z-z_*)+(z-z_*)r(z),\qquad r(z)\to0.
$$

The first two terms have polynomial primitives, hence integrate to zero around each triangle. For sufficiently large $n$, $|r|<\varepsilon$ on $T_n$, so the [complex line integral estimate](../../../../../../complex-line-integral-estimate.md) gives

$$
\left|\int_{\partial T_n}f(z)\,dz\right|\leq\varepsilon d_nP_n.
$$

Combining the bounds gives $|\int_{\partial T}f(z)\,dz|\leq\varepsilon d_0P_0$. Since $\varepsilon$ is arbitrary,

$$
\boxed{\int_{\partial T}f(z)\,dz=0.}
$$

The orientation can be reversed with no change to the conclusion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13G](../../13g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

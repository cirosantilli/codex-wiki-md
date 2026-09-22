<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [linear operator](../../../../../../linear-operator.md) on finite-dimensional vectors acts by $(Au)_i=\sum_jA_{ij}u_j$. For a field the discrete index becomes a continuous coordinate, and a suitable operator is represented by an [integral kernel](../../../../../../integral-kernel.md), possibly a [distribution](../../../../../../distribution-mathematical-analysis.md):

$$
(A\phi)(x)=\int d^dy\,A(x,y)\phi(y),\qquad
(AB)(x,y)=\int d^dz\,A(x,z)B(z,y).
$$

The [identity operator](../../../../../../identity-operator.md) has kernel $\delta^{(d)}(x-y)$. If an inverse exists on the chosen domain and with the chosen boundary prescription, its kernel satisfies

$$
\boxed{\int d^dz\,A(x,z)A^{-1}(z,y)=\delta^{(d)}(x-y),}
$$

with the analogous reversed identity. A differential operator is a distributional kernel: for example, $A(x,y)=(-\Box_x-m^2)\delta^{(d)}(x-y)$. Its inverse is a [Green function](../../../../../../green-s-function.md). Boundary conditions, a causal prescription and the treatment of zero modes are part of the inverse's definition, not consequences of formal matrix notation. An operator with an untreated zero mode does not have an inverse on the full field space.

The [functional derivative](../../../../../../functional-derivative.md) is defined through the [first variation](../../../../../../first-variation.md): for arbitrary smooth test variation $h$,

$$
F[\phi+\varepsilon h]-F[\phi]
=\varepsilon\int d^dx\,\frac{\delta F}{\delta\phi(x)}h(x)+o(\varepsilon).
$$

In particular,

$$
\frac{\delta\phi(x)}{\delta\phi(y)}=\delta^{(d)}(x-y),\qquad
\frac{\delta}{\delta\phi(y)}\int d^dx\,J(x)\phi(x)=J(y).
$$

For a symmetric kernel, differentiating $F[\phi]=\tfrac12\int dx\,dy\,\phi(x)A(x,y)\phi(y)$ gives $\delta F/\delta\phi=A\phi$. The two terms from varying the two fields coincide; for a nonsymmetric kernel the symmetric part $(A+A^T)/2$ appears instead. [Integration by parts](../../../../../../integration-by-parts.md) is understood when $A$ is differential and the boundary variations vanish. A finite-volume, finite-mode regulator makes these statements ordinary matrix identities before a continuum limit.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

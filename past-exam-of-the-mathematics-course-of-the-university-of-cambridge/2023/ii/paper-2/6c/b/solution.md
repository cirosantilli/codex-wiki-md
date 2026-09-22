<h1 id="6c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At a nontrivial equilibrium $I^*>0$, the equation $I'=0$ gives

$$
S^*=\frac\nu\beta.
$$

The equation $R'=0$ gives $R^*=\nu I^*/f$, and conservation of population then yields

$$
I^*=\frac{f(\beta N-\nu)}{\beta(f+\nu)},
\qquad
R^*=\frac{\nu(\beta N-\nu)}{\beta(f+\nu)}.
$$

These values are positive precisely in the epidemic regime $\beta N>\nu$.

Eliminate $R=N-S-I$. The two-dimensional system is

$$
S'=f(N-S-I)-\beta IS,
\qquad
I'=(\beta S-\nu)I.
$$

Set $a=\beta I^*=f(\beta N-\nu)/(f+\nu)>0$. The [Jacobian matrix](../../../../../../jacobian-matrix.md) at the endemic equilibrium is

$$
J=
\begin{pmatrix}
-(f+a)&-(f+\nu)\\
a&0
\end{pmatrix},
$$

so its eigenvalues satisfy

$$
\lambda^2+(f+a)\lambda+a(f+\nu)=0.
$$

Their sum is $-(f+a)<0$ and their product is $a(f+\nu)>0$, proving [local asymptotic stability](../../../../../../linear-stability-of-a-planar-equilibrium.md).

The discriminant is

$$
\Delta=(f+a)^2-4a(f+\nu).
$$

Writing $r=\beta N-\nu>0$, we have $a=fr/(f+\nu)$. As $f\to0^+$,

$$
\Delta=-4fr+O(f^2)<0,
$$

whereas as $f\to\infty$,

$$
\Delta=f^2-2rf+O(1)>0.
$$

Hence sufficiently slow immunity loss gives a stable focus: $I(t)$ approaches $I^*$ through damped oscillations, corresponding to successively smaller epidemic waves. Sufficiently rapid immunity loss gives a stable node: small disturbances are sums of two decaying real modes and show no forced oscillation. These conclusions and the equilibrium formulas are collected in the [Endemic equilibrium of the SIR model with waning immunity](../../../../../../endemic-equilibrium-of-the-sir-model-with-waning-immunity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6C](../../6c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

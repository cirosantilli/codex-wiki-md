<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $\alpha=2$, part iii gives $a=1$, $b=2$, and $\beta=1$. Put

$$
H=tF(\eta),
\qquad
\eta=\frac{x}{t^2},
\qquad
x_N(t)=\eta_Nt^2.
$$

Substitution into the nonlinear [partial differential equation](../../../../../../partial-differential-equation-split.md) gives the [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\boxed{
A(F^3F')'+2\eta F'-F-D=0}
$$

with [boundary conditions](../../../../../../boundary-condition.md)

$$
\boxed{-AF(0)^3F'(0)=Q_0,
\qquad F(\eta_N)=0,
\qquad F^3F'\longrightarrow0
\ \text{as }\eta\uparrow\eta_N}.
$$

To find the leading edge, set $y=\eta_N-\eta$ and suppose $F\sim Cy^p$. The two singular terms in the [ordinary differential equation](../../../../../../ordinary-differential-equation.md) have orders $y^{4p-2}$ and $y^{p-1}$. Their exponents agree only when $p=1/3$. Their leading coefficients then satisfy

$$
\frac{AC^4}{9}-\frac{2\eta_NC}{3}=0,
$$

whereas $F$ and the constant drainage $D$ are lower-order terms. Hence

$$
\boxed{
F(\eta)\sim
\left(\frac{6\eta_N}{A}\right)^{1/3}
(\eta_N-\eta)^{1/3}}
\qquad(\eta\uparrow\eta_N).
$$

The [draining gravity current](../../../../../../draining-gravity-current.md) therefore has a one-third-power leading edge and its flux vanishes there.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

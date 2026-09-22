<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $I_b,I_f$ count internal scalar and fermion lines and $L$ count independent loops in a connected amputated [Feynman diagram](../../../../feynman-diagram.md). At large [loop momentum](../../../../loop-momentum.md), the [scalar propagator](../../../../scalar-propagator.md) falls as $k^{-2}$ and the [Dirac propagator](../../../../dirac-propagator.md) falls as $k^{-1}$, including its numerator. Each loop integration is $d^3k$. The nonderivative [interaction vertices](../../../../interaction-vertex.md) add no powers. Therefore

$$
\omega=3L-2I_b-I_f.
$$

Count endpoints of each kind of line and use the connected-graph [loop order](../../../../loop-order.md) identity:

$$
2I_b+b=2n_1+4n_2+6n_3,\qquad
2I_f+f=2n_1,\qquad
L=I_b+I_f-(n_1+n_2+n_3)+1.
$$

Eliminating $L,I_b,I_f$ gives

$$
\begin{aligned}
\omega&=I_b+2I_f-3(n_1+n_2+n_3)+3\\
&=\left(n_1+2n_2+3n_3-\frac b2\right)+2\left(n_1-\frac f2\right)-3(n_1+n_2+n_3)+3\\
&=\boxed{3-\frac b2-f-n_2.}
\end{aligned}
$$

The cancellation of $n_1,n_3$ reflects their dimensionless couplings; every insertion of the positive-dimensional $g_2$ improves the [superficial degree of divergence](../../../../superficial-degree-of-divergence.md) by one.

The printed exact homogeneity is shorthand for ultraviolet [power counting](../../../../power-counting-in-quantum-field-theory.md), not an identity for a massive integrated [correlation function](../../../../correlation-function.md). For example, even the free amputated scalar two-point vertex $\Gamma^{(2)}(p)=p^2-M^2$ obeys $\Gamma^{(2)}(\lambda p)=\lambda^2p^2-M^2$, which differs from $\lambda^2\Gamma^{(2)}(p)$ when $M\ne0$. [Logarithmic divergences](../../../../logarithmic-divergence.md), actual numerator cancellations and [ultraviolet subdivergences](../../../../ultraviolet-subdivergence.md) also require separate treatment.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

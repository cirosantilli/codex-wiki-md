<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h_{ij}={}^{(3)}g_{ij}$ for the [induced metric](../../../../../../induced-metric.md) and lower the [shift vector](../../../../../../shift-vector.md) with it, $N_i=h_{ij}N^j$. In the stated negative-shift convention the four-dimensional components and inverse components are

$$
g_{00}=-N^2+N_iN^i,\quad g_{0i}=-N_i,\quad g_{ij}=h_{ij},
\qquad g^{00}=-\frac1{N^2},\quad g^{0i}=-\frac{N^i}{N^2}.
$$

Multiplying the given future [unit normal](../../../../../../unit-normal.md) by this [metric tensor](../../../../../../metric-tensor.md) gives $n_\mu=(-N,0,0,0)$. In particular the tangential normal components vanish, but their [covariant derivatives](../../../../../../covariant-derivative.md) do not:

$$
n_{i;j}=-\Gamma^\mu{}_{ij}n_\mu=N\Gamma^0{}_{ij},\qquad K_{ij}=-N\Gamma^0{}_{ij}.
$$

The relevant [Christoffel symbol](../../../../../../christoffel-symbol.md) is

$$
\begin{aligned}
\Gamma^0{}_{ij}
&=\frac1{2N^2}\left[\dot h_{ij}+\partial_iN_j+\partial_jN_i
-N^k(\partial_i h_{jk}+\partial_jh_{ik}-\partial_kh_{ij})\right]\\
&=\frac1{2N^2}\left(\dot h_{ij}+N_{i|j}+N_{j|i}\right).
\end{aligned}
$$

For the second equality, the last parenthesis is $2h_{k\ell}{}^{(3)}\Gamma^\ell{}_{ij}$, so its contraction subtracts the two spatial connection terms in the symmetrized derivative of $N_i$. Therefore

$$
\boxed{K_{ij}=-\frac1{2N}\left(\dot h_{ij}+N_{i|j}+N_{j|i}\right).}
$$

This is [extrinsic curvature with a negative shift](../../../../../../extrinsic-curvature-with-a-negative-shift.md). Both the future-normal orientation and the definition $K=-\nabla n$ matter: replacing the threading by $dx^i+N^idt$ reverses the shift terms. The spatial [induced metric](../../../../../../induced-metric.md) is generally a function of time as well as position; restricting it to time-independent data would simply make the displayed time derivative vanish.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

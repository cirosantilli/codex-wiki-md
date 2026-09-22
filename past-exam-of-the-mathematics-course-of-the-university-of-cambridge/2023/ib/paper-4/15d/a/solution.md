<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $[AB,C]=A[B,C]+[A,C]B$ and the [canonical commutation relation](../../../../../../canonical-commutation-relation.md). With $L_i=\varepsilon_{iab}x_ap_b$,

$$
\begin{aligned}
[L_i,x_j]
&=\varepsilon_{iab}x_a[p_b,x_j]
=-i\hbar\varepsilon_{iaj}x_a
=i\hbar\varepsilon_{ijk}x_k,\\
[L_i,p_j]
&=\varepsilon_{iab}[x_a,p_j]p_b
=i\hbar\varepsilon_{ijb}p_b
=i\hbar\varepsilon_{ijk}p_k.
\end{aligned}
$$

Using these two transformation laws on $L_j=\varepsilon_{jab}x_ap_b$ gives

$$
\begin{aligned}
[L_i,L_j]
&=\varepsilon_{jab}([L_i,x_a]p_b+x_a[L_i,p_b])\\
&=\boxed{i\hbar\varepsilon_{ijk}L_k}.
\end{aligned}
$$

These are the [orbital angular momentum commutation relations](../../../../../../orbital-angular-momentum-commutation-relations.md).

Now

$$
[L^2,L_i]=\sum_j\bigl(L_j[L_j,L_i]+[L_j,L_i]L_j).
$$

The factor $[L_j,L_i]$ is antisymmetric in $j$ and its remaining product is symmetric after the two terms are combined, so the contraction vanishes:

$$
\boxed{[L^2,L_i]=0}.
$$

The same commutators show that $p^2=p_jp_j$ and $r^2=x_jx_j$ are rotational scalars: their commutators with every $L_i$ vanish by contraction of the antisymmetric $\varepsilon_{ijk}$ with a symmetric product. Therefore $U(r)$ also commutes with every $L_i$, and for

$$
H=\frac{p^2}{2m}+U(r)
$$

we have $[H,L_i]=0$, hence

$$
\boxed{[H,L^2]=0}.
$$

In particular $H,L^2,L_3$ are pairwise commuting Hermitian operators. By [simultaneous diagonalization](../../../../../../simultaneous-diagonalization.md), they admit a common eigenbasis, subject to the usual spectral-domain qualifications for unbounded operators. This is the [rotational invariance of a central-potential Hamiltonian](../../../../../../rotational-invariance-of-a-central-potential-hamiltonian.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

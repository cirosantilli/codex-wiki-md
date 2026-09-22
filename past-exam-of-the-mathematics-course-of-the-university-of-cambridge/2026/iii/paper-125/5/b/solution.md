<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Q\in E'[\widehat\phi]$. The compatibility of divisor classes with pullback identifies the class of

$$
\phi^*((Q)-(O))
$$

with $\widehat\phi(Q)=O$, so choose $g_Q\in K(E)^\times$ with

$$
\operatorname{div}(g_Q)=\phi^*((Q)-(O)).
$$

Since $[n]Q=\phi\widehat\phi(Q)=O$, choose $f_Q\in K(E')^\times$ with

$$
\operatorname{div}(f_Q)=n((Q)-(O)).
$$

The functions $f_Q\circ\phi$ and $g_Q^n$ have the same divisor. Their quotient is constant, and because $K$ is algebraically closed we may rescale $g_Q$ so that

$$
f_Q\circ\phi=g_Q^n.
$$

Thus define

$$
E'[\widehat\phi]\longrightarrow
\frac{K(E')^\times\cap K(E)^{\times n}}{K(E')^{\times n}},
\qquad Q\longmapsto[f_Q].
$$

Changing either function changes $f_Q$ only by an $n$th power of a constant. The divisor relation for $Q+R$ differs from the sum of those for $Q$ and $R$ by $n$ times a principal divisor, so the map is a homomorphism. If $[f_Q]$ is trivial, then $f_Q=h^n$ for $h\in K(E')^\times$, whence $\operatorname{div}(h)=(Q)-(O)$; the divisor-class isomorphism forces $Q=O$. The map is therefore well-defined and injective.

For $P\in E[\phi]$, translation by $P$ fixes $g_Q^n=f_Q\circ\phi$. Hence

$$
e_\phi(P,Q)=\frac{g_Q(X+P)}{g_Q(X)}\in\mu_n
$$

is independent of the auxiliary point $X$. This is the [Weil pairing](../../../../../../weil-pairing.md) associated with $\phi$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

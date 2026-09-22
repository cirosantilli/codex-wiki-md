<h1 id="22h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose $a^k\rightharpoonup a$ in $\ell^1$ but $a^k$ does not converge to $a$ in the [norm topology](../../../../../../norm-topology.md). There are $\varepsilon>0$ and a [subsequence](../../../../../../subsequence.md) $(a^{m_k})$ such that

$$
\lVert a^{m_k}-a\rVert_1\geq\varepsilon
\qquad\text{for every }k.
$$

Set $x^k=a^{m_k}-a$. Then

$$
x^k\rightharpoonup0,
\qquad \lVert x^k\rVert_1\geq\varepsilon,
$$

which proves the first assertion.

We now use a [gliding hump argument](../../../../../../gliding-hump-argument.md). Put $b_0=0$. Having chosen $b_{n-1}$ and $k_{n-1}$, coordinatewise convergence $x_i^k\to0$ lets us choose $k_n>k_{n-1}$ so that

$$
A_n:=\sum_{i\leq b_{n-1}}|x_i^{k_n}|<\frac\varepsilon6.
$$

For this fixed element of $\ell^1$, choose $b_n>b_{n-1}$ so far out that

$$
C_n:=\sum_{i>b_n}|x_i^{k_n}|<\frac\varepsilon6.
$$

Define one sequence $y$ by

$$
y_i=\operatorname{sgn}(x_i^{k_n})
\qquad\text{when }b_{n-1}<i\leq b_n.
$$

The blocks partition the positive integers and $|y_i|\leq1$, so $y\in\ell^\infty$. On the $n$th assigned block, the signs agree; outside it, use $|y_i|\leq1$. The [duality of l1 and l infinity](../../../../../../duality-of-l1-and-l-infinity.md) gives

$$
\begin{aligned}
\langle x^{k_n},y\rangle
&\geq
\sum_{b_{n-1}<i\leq b_n}|x_i^{k_n}|-A_n-C_n\\
&=\lVert x^{k_n}\rVert_1-2A_n-2C_n\\
&>\varepsilon-\frac{2\varepsilon}{6}-\frac{2\varepsilon}{6}
=\frac\varepsilon3.
\end{aligned}
$$

But $x^{k_n}\rightharpoonup0$ requires $\langle x^{k_n},y\rangle\to0$ for this fixed $y\in(\ell^1)^*=\ell^\infty$, a contradiction. Therefore every weakly convergent sequence in $\ell^1$ converges in norm. This is the [Schur property of l1](../../../../../../schur-property-of-l1.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22H](../../22h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

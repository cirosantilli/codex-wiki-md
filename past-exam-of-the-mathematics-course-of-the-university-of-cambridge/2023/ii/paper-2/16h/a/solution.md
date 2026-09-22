<h1 id="16h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero [ordinal](../../../../../../ordinal.md) $\alpha$, let

$$
S=\{\xi:\omega^\xi\leq\alpha\}.
$$

The set is nonempty because $0\in S$, and it is an initial segment because [ordinal exponentiation](../../../../../../ordinal-exponentiation.md) by $\omega$ is strictly increasing. Put $\beta=\sup S$.

If $\beta$ is a successor, the definition of the [supremum](../../../../../../supremum.md) forces $\beta\in S$. If $\beta$ is a [limit ordinal](../../../../../../limit-ordinal.md), then continuity of ordinal exponentiation gives

$$
\omega^\beta
=\sup_{\xi<\beta}\omega^\xi
\leq\alpha,
$$

so again $\beta\in S$. Thus $\omega^\beta\leq\alpha$, while $\omega^{\beta+1}>\alpha$ by the definition of the supremum. Hence $\beta$ is the greatest required exponent.

Apply [division by an additively indecomposable ordinal](../../../../../../division-by-an-additively-indecomposable-ordinal.md) with $\lambda=\omega^\beta$:

$$
\alpha=\omega^\beta q+\gamma,
\qquad
\gamma<\omega^\beta.
$$

Since $\alpha\geq\omega^\beta$, the quotient $q$ is nonzero. It must be finite: if $q\geq\omega$, then

$$
\omega^{\beta+1}
=\omega^\beta\omega
\leq\omega^\beta q
\leq\alpha,
$$

contradicting the maximality of $\beta$. Writing $q=n$ gives

$$
\boxed{\alpha=\omega^\beta n+\gamma},
\qquad
0<n<\omega,\quad \gamma<\omega^\beta.
$$

This is the [leading-term decomposition](../../../../../../greatest-power-of-omega-below-an-ordinal.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16H](../../16h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

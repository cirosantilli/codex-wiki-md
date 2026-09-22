<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\sigma>1$, [Orthogonality of Dirichlet characters](../../../../../../orthogonality-of-dirichlet-characters.md) gives

$$
\sum_{\substack{n\geq1\\n\equiv a\pmod q}}
\frac{\Lambda(n)}{n^\sigma}
=\frac1{\varphi(q)}
\sum_{\chi\bmod q}\overline{\chi(a)}
\left(-\frac{L'(\sigma,\chi)}{L(\sigma,\chi)}\right).
$$

The principal-character term is

$$
\frac1{\sigma-1}+O_q(1).
$$

Part (a) makes every nonprincipal logarithmic derivative bounded as $\sigma\to1^+$, so

$$
\sum_{\substack{n\geq1\\n\equiv a\pmod q}}
\frac{\Lambda(n)}{n^\sigma}
=\frac1{\varphi(q)(\sigma-1)}+O_q(1)
\longrightarrow\infty.
$$

If the nondecreasing [Chebyshev function in an arithmetic progression](../../../../../../chebyshev-function-in-an-arithmetic-progression.md)

$$
\psi(x;q,a)=\sum_{\substack{n\leq x\\n\equiv a\pmod q}}\Lambda(n)
$$

were bounded, the [Abel summation formula](../../../../../../abel-s-summation-formula.md) would keep the displayed Dirichlet series bounded near $\sigma=1$. Therefore

$$
\boxed{\psi(x;q,a)\longrightarrow\infty.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

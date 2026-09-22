<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For stationary edge flow $Q(x,y)=\pi^G(x)P(x,y)$, the [bottleneck ratio](../../../../../../conductance-of-a-markov-chain.md) is

$$
\Phi_*^G
=\min_{0<\pi^G(S)\leq1/2}
\frac{Q(S,S^c)}{\pi^G(S)}.
$$

Using $f=\mathbf1_S$ in the variational characterization,

$$
\gamma^G
\leq\frac{\mathcal E(f,f)}{\operatorname{Var}_{\pi^G}f}
=\frac{Q(S,S^c)}{\pi^G(S)\pi^G(S^c)}
\leq2\frac{Q(S,S^c)}{\pi^G(S)}.
$$

Taking the infimum gives $\gamma^G\leq2\Phi_*^G$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

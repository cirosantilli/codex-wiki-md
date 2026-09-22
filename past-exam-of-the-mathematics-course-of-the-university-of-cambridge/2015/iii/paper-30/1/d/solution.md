<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use deterministic times tending to infinity and the [Fatou lemma](../../../../../../fatou-s-lemma.md):

$$
\boxed{D:=\mathbb E[e^{M_\infty/2}]
\leq\liminf_{n\to\infty}\mathbb E[e^{M_n/2}]
\leq K<\infty.}
$$

Apply the [terminal scaling inequality for stochastic exponentials](../../../../../../terminal-scaling-inequality-for-stochastic-exponentials.md) to $X=aM$ and $r=1/a$. Part (c) gives $\mathbb E[\mathcal E(aM)_\infty]=1$, so

$$
\mathbb E[\mathcal E(M)_\infty]\geq D^{-2(1/a-1)}.
$$

Letting $a\uparrow1$ shows that the terminal expectation is at least one. The [nonnegative local martingale](../../../../../../nonnegative-local-martingale.md) $\mathcal E(M)$ starts at one and is a [supermartingale](../../../../../../supermartingale.md), so the [Fatou lemma](../../../../../../fatou-s-lemma.md) gives the opposite inequality. Consequently

$$
\boxed{\mathbb E[\mathcal E(M)_\infty]=1.}
$$

The [terminal expectation criterion for a nonnegative local martingale](../../../../../../terminal-expectation-criterion-for-a-nonnegative-local-martingale.md) now closes the argument. Conditional [Fatou lemma](../../../../../../fatou-s-lemma.md) applied to the [supermartingale](../../../../../../supermartingale.md) at times tending to infinity gives

$$
\mathbb E[\mathcal E(M)_\infty\mid\mathcal F_t]\leq\mathcal E(M)_t.
$$

The left side has expectation one and the right side at most one, so equality holds almost surely. Thus

$$
\boxed{\mathcal E(M)_t
=\mathbb E[\mathcal E(M)_\infty\mid\mathcal F_t],}
$$

and [uniform integrability of conditional expectations](../../../../../../uniform-integrability-of-conditional-expectations.md) proves that $\mathcal E(M)$ is a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md). This establishes the required stopped-moment form of the [Kazamaki criterion](../../../../../../kazamaki-s-condition.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

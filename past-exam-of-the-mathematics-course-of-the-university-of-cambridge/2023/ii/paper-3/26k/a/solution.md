<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $T$ be a [measure-preserving transformation](../../../../../../measure-preserving-transformation.md) of $(X,\mathcal F,\mu)$ and let $f\in L^1(\mu)$. The [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md) states that

$$
A_nf:=\frac1n\sum_{j=0}^{n-1}f\circ T^j
\longrightarrow
f^*:=\mathbb E[f\mid\mathcal I]
$$

almost everywhere, where $\mathcal I$ is the [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md). The limit is $T$-invariant and

$$
\int_Xf^*,d\mu=\int_Xf,d\mu.
$$

Assume now that $\mu(X)=1$. For $M>0$, let

$$
f_M=(-M)\vee(f\wedge M)
$$

be the bounded truncation of $f$, and let $f_M^*$ be its Birkhoff limit. Since $|A_nf_M-f_M^*|\leq2M$ on a [finite measure](../../../../../../finite-measure.md) space, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\|A_nf_M-f_M^*\|_1\longrightarrow0.
$$

Measure preservation and the [triangle inequality](../../../../../../triangle-inequality.md) give the $L^1$ contraction

$$
\|A_nh\|_1
\leq\frac1n\sum_{j=0}^{n-1}\|h\circ T^j\|_1
=\|h\|_1.
$$

Moreover, the almost-everywhere convergence and [Fatou lemma](../../../../../../fatou-s-lemma.md) imply

$$
\|f^*-f_M^*\|_1
\leq\liminf_{n\to\infty}\|A_n(f-f_M)\|_1
\leq\|f-f_M\|_1.
$$

Consequently

$$
\limsup_{n\to\infty}\|A_nf-f^*\|_1
\leq2\|f-f_M\|_1.
$$

Since $f_M\to f$ in $L^1$, letting $M\to\infty$ proves the [L1 convergence in the Birkhoff ergodic theorem on a finite measure space](../../../../../../l1-convergence-in-the-birkhoff-ergodic-theorem-on-a-finite-measure-space.md):

$$
\boxed{A_nf\longrightarrow f^*\quad\hbox{in }L^1(\mu).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

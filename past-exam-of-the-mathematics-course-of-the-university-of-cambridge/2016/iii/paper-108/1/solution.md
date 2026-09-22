<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work with a probability [measure-preserving system](../../../../../measure-preserving-system.md), so $\mu(X)=1$. Put

$$
S_nf=\sum_{j=0}^{n-1}f\circ T^j,\qquad A_nf=\frac{S_nf}{n}.
$$

The **maximal ergodic theorem**, also called the [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md), says that for real $f\in L^1(\mu)$,

$$
E_N=\{\max_{1\leq n\leq N}S_nf>0\},\qquad E=\{\sup_{n\geq1}S_nf>0\}
\quad\Longrightarrow\quad
\boxed{\int_{E_N}f\,d\mu\geq0,\qquad\int_Ef\,d\mu\geq0.}
$$

No [ergodic transformation](../../../../../ergodicity.md) or invertibility assumption is needed for this [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md).

Here is a proof of the [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md). Set $M_0=0$ and $M_N=\max(0,S_1f,\ldots,S_Nf)$. These are integrable: $0\leq M_N\leq\sum_{j=0}^{N-1}|f|\circ T^j$. Splitting off the first summand gives

$$
M_N=\max(0,f+M_{N-1}\circ T),\qquad M_{N-1}\leq M_N.
$$

On $E_N=\{M_N>0\}$, this implies $f=M_N-M_{N-1}\circ T\geq M_N-M_N\circ T$. Outside $E_N$ the right side is $-M_N\circ T\leq0$. Consequently

$$
f\mathbf1_{E_N}\geq M_N-M_N\circ T.
$$

Integrating and using the [measure-preserving transformation](../../../../../measure-preserving-transformation.md) property gives $\int_{E_N}f\,d\mu\geq0$. Since $E_N$ increases to $E$, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), with dominating function $|f|$, proves the infinite-supremum assertion of the [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md).

For example, applying the [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md) to $|f|-\varepsilon$ yields the useful maximal bound

$$
\mu\{\sup_{n\geq1}|A_nf|>\varepsilon\}
\leq\mu\{\sup_{n\geq1}A_n|f|>\varepsilon\}
\leq\frac{\|f\|_1}{\varepsilon}\qquad(\varepsilon>0).
$$

Indeed on the latter set $G$, the [maximal ergodic lemma](../../../../../maximal-ergodic-lemma.md) gives $\varepsilon\mu(G)\leq\int_G|f|\,d\mu$.

The **[pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md)** states that for a probability [measure-preserving system](../../../../../measure-preserving-system.md) and $f\in L^1(\mu)$,

$$
\boxed{A_nf\longrightarrow\mathbb E[f\mid\mathcal I]\quad\text{almost everywhere},}
$$

where $\mathcal I$ is the [invariant sigma-algebra](../../../../../invariant-sigma-algebra.md). The [conditional expectation](../../../../../conditional-expectation.md) is invariant and has integral $\int f\,d\mu$. If $T$ is an [ergodic transformation](../../../../../ergodicity.md), this [conditional expectation](../../../../../conditional-expectation.md) is the constant $\int f\,d\mu$. The assertion applies to real or complex integrable functions; it is the [Birkhoff ergodic theorem](../../../../../birkhoff-ergodic-theorem.md).

For a nonnegative measurable $f$, if $\int f\,d\mu<\infty$, the [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) already proves the required conclusion. For the remaining case, let $f_K=\min(f,K)$, $K=1,2,\ldots$. Each $f_K$ is integrable on the probability [measure-preserving system](../../../../../measure-preserving-system.md). The [pointwise ergodic theorem](../../../../../birkhoff-ergodic-theorem.md) and [ergodic transformation](../../../../../ergodicity.md) property give, on a single set of full measure obtained by a countable intersection,

$$
\lim_{n\to\infty}A_nf_K(x)=\int f_K\,d\mu\qquad\text{for every }K.
$$

Since $f\geq f_K$, every such $x$ satisfies $\liminf_n A_nf(x)\geq\int f_K\,d\mu$ for all $K$. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives $\int f_K\,d\mu\uparrow\int f\,d\mu=+\infty$. Thus the [nonnegative ergodic averages with infinite integral](../../../../../nonnegative-ergodic-averages-with-infinite-integral.md) tend to $+\infty$, rather than merely having an unbounded subsequence. Combining the two cases,

$$
\boxed{\lim_{n\to\infty}\frac1n\sum_{j=0}^{n-1}f(T^jx)=\int f\,d\mu\in[0,+\infty]\quad\text{almost everywhere}.}
$$

Nonnegativity is what makes truncation a lower bound. The probability normalization is also essential to the displayed value: for a finite measure of total mass $c>0$, the corresponding constant is $c^{-1}\int f\,d\mu$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

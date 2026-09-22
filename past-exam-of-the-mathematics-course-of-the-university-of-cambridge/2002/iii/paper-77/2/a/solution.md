<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the positive-integer [geometric distribution](../../../../../../geometric-distribution.md), $\mathbb P(X=k)=p(1-p)^{k-1}$ for $k\geq1$, initially with $0<p<1$. Put $a=-\log(1-p)>0$. The precise [good rate function](../../../../../../good-rate-function.md) on $\mathbb R$ is

$$
\boxed{I(x)=
\begin{cases}
ax,&x\geq0,\\
+\infty,&x<0.
\end{cases}}
$$

The [large-deviation speed](../../../../../../large-deviation-speed.md) is $L\to\infty$. We prove both bounds of the [large deviation principle](../../../../../../large-deviation-principle.md) for $X^L=X/L$.

For $x>0$, the geometric tail gives the exact expression

$$
\mathbb P(X^L\geq x)
=(1-p)^{\lceil Lx\rceil-1},
\qquad
\lim_{L\to\infty}L^{-1}\log\mathbb P(X^L\geq x)=-ax.
$$

Let $F$ be a [closed set](../../../../../../closed-set.md). If it does not meet $[0,\infty)$ its probability is zero. If it contains zero, $\limsup L^{-1}\log\mathbb P(X^L\in F)\leq0=-\inf_FI$. Otherwise, if it meets the nonnegative half-line, its least possible nonnegative value $r$ is positive: a sequence in $F$ approaching zero would force zero into the closed set. Its event is contained in $\{X^L\geq r\}$, giving

$$
\limsup_{L\to\infty}L^{-1}\log\mathbb P(X^L\in F)
\leq-ar=-\inf_FI.
$$

For an [open set](../../../../../../open-set.md) $G$ containing $x>0$, choose positive integers $k_L$ with $k_L/L\to x$. Eventually $k_L/L\in G$, and

$$
\liminf_{L\to\infty}L^{-1}\log\mathbb P(X^L\in G)
\geq\lim_{L\to\infty}L^{-1}\log[p(1-p)^{k_L-1}]
=-ax.
$$

If $0\in G$, the event $X=1$ alone gives lower exponential rate zero; alternatively the probability of a neighborhood of zero tends to one. Optimizing over $x\in G$ proves the open-set lower bound. Sets containing no nonnegative point require only the trivial lower bound $-\infty$.

The [rate function](../../../../../../rate-function.md) is [lower semicontinuous](../../../../../../lower-semicontinuity.md) at zero as well as elsewhere, and $\{I\leq r\}=[0,r/a]$ for finite $r\geq0$ is [compact](../../../../../../compact-space.md). Hence the [large deviation principle](../../../../../../large-deviation-principle.md) has a [good rate function](../../../../../../good-rate-function.md). This establishes the [large deviations of a scaled geometric random variable](../../../../../../large-deviations-of-a-scaled-geometric-random-variable.md). For $p=1$, $X=1$ deterministically and the rate instead is zero at $x=0$ and infinite elsewhere; the displayed logarithmic coefficient must not be treated as an ordinary finite number in that case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

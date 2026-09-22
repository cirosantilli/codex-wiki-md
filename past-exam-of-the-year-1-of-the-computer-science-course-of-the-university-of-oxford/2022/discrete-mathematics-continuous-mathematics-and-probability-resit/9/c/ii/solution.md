<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $W_i=U_i^2$. Applying the same [measurable function](../../../../../../measurable-function.md) separately to [independent and identically distributed](../../../../../../independent-and-identically-distributed-random-variables.md) [random variables](../../../../../../random-variable-split.md) preserves those two properties, and

$$
\mathbb E[W_i]=\int_0^1u^2\,\mathrm du=\frac13.
$$

In particular, these bounded [random variables](../../../../../../random-variable-split.md) are [integrable random variables](../../../../../../integrable-random-variable.md). The [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives

$$
\overline W_n=\frac1n\sum_{i=1}^nW_i\xrightarrow{\mathbb P}\frac13.
$$

If $c>1/3$, then $\{\overline W_n>c\}\subseteq\{|\overline W_n-1/3|\geqslant c-1/3\}$, whose [probability](../../../../../../probability.md) tends to zero. If $0\leqslant c<1/3$, then $\{\overline W_n\leqslant c\}\subseteq\{|\overline W_n-1/3|\geqslant1/3-c\}$, whose [probability](../../../../../../probability.md) also tends to zero. Taking a complement in the second case proves

$$
\boxed{\mathbb P\!\left(\sum_{i=1}^nU_i^2>cn\right)\longrightarrow\begin{cases}0,&c>1/3,\\1,&0\leqslant c<1/3.\end{cases}}
$$

The positive gap from $1/3$ is essential to this argument. [Convergence in probability](../../../../../../convergence-in-probability.md) alone does not determine the answer at the excluded threshold $c=1/3$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

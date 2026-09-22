<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First take $0<p<1$. For $X\sim\operatorname{Bin}(n,p)$, [independence](../../../../../independent-random-variables.md) of the Bernoulli trials gives

$$
\mathbb E(e^{tX})=(1-p+pe^t)^n.
$$

For $x\geq p$ and $t>0$, [Markov inequality](../../../../../markov-s-inequality.md) yields

$$
P(X\geq nx)\leq e^{-tnx}(1-p+pe^t)^n.
$$

Differentiate the logarithm of the right-hand side to minimize it. The stationary point satisfies

$$
e^{t_*}=\frac{x(1-p)}{p(1-x)},
$$

which is at least $1$ when $x\geq p$. Substitution gives

$$
\boxed{P(X\geq nx)\leq
\left[\left(\frac px\right)^x\left(\frac{1-p}{1-x}\right)^{1-x}\right]^n.}
$$

When $x=p$, use the limit $t_*\to0$, giving the trivial bound $1$.

For $x\leq p$, take $t<0$. On $\{X\leq nx\}$ we have $e^{tX}\geq e^{tnx}$, so the same [Markov inequality](../../../../../markov-s-inequality.md) gives the same expression. Its minimizing $t_*$ is now nonpositive, yielding the stated lower-tail bound. No rounding of $nx$ is needed, because the exponential event inclusion holds for real thresholds. The cases $p=0$ and $p=1$ are deterministic and follow directly, or by the corresponding limits.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

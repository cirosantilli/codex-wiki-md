<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $t>e$, put $\Phi(t)=\sqrt{2t\log\log t}$. Fix $a>1$ and $\varepsilon>0$, and set

$$
E_n=\left\{\sup_{0\leq s\leq a^n}B_s
\geq(1+\varepsilon)\Phi(a^n)\right\}
$$

for $n$ large enough that $a^n>e$. The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) and the Gaussian tail estimate give

$$
\begin{aligned}
\mathbb P(E_n)
&=2\mathbb P\left(B_{a^n}\geq(1+\varepsilon)\Phi(a^n)\right)\\
&\leq2\exp\bigl(-(1+\varepsilon)^2\log\log(a^n)\bigr)\\
&=2(n\log a)^{-(1+\varepsilon)^2}.
\end{aligned}
$$

Since $(1+\varepsilon)^2>1$, the sum of these probabilities is finite. The [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md) implies that, [almost surely](../../../../../../almost-sure-convergence.md), for all sufficiently large $n$,

$$
\sup_{s\leq a^n}B_s<(1+\varepsilon)\Phi(a^n).
$$

Now take $t\in[a^{n-1},a^n]$. The function $\Phi$ is increasing for $t>e$, so

$$
\frac{B_t}{\Phi(t)}
\leq(1+\varepsilon)\frac{\Phi(a^n)}{\Phi(a^{n-1})}.
$$

Here the positive upper bound for $B_t$ can first be divided by $\Phi(t)$, and the denominator can then be bounded below by $\Phi(a^{n-1})$; this remains valid even when $B_t<0$. Moreover,

$$
\frac{\Phi(a^n)}{\Phi(a^{n-1})}
=\sqrt{a\,\frac{\log(n\log a)}{\log((n-1)\log a)}}
\longrightarrow\sqrt a.
$$

Thus, for each fixed pair $(a,\varepsilon)$,

$$
\limsup_{t\to\infty}\frac{B_t}{\Phi(t)}
\leq(1+\varepsilon)\sqrt a
\quad\text{almost surely}.
$$

Use the countable choices $a_m=1+1/m$ and $\varepsilon_m=1/m$, intersect their probability-one events, and let $m\to\infty$. This proves the [Brownian upper law of the iterated logarithm](../../../../../../brownian-upper-law-of-the-iterated-logarithm.md):

$$
\boxed{\limsup_{t\to\infty}\frac{B_t}{\sqrt{2t\log\log t}}
\leq1\quad\text{almost surely}.}
$$

Only large times are involved. The hint's related monotonicity assertion for $\Phi(t)/t$ is also valid eventually: the derivative of $2\log\log t/t$ is $2(1/\log t-\log\log t)/t^2$, which is negative for $t\geq e^e$. No monotonicity at the small-time edge of the logarithmic expression is required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

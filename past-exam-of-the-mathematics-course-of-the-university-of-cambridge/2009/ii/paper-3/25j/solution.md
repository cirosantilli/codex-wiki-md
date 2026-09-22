<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

For events $A_n$, their limsup is the event that infinitely many occur. The first [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) states that $\sum_n\mathbb P(A_n)<\infty$ implies $\mathbb P(\limsup A_n)=0$, without independence. Indeed

$$
\mathbb P\!\left(\bigcup_{n\ge N}A_n\right)\le\sum_{n\ge N}\mathbb P(A_n)\longrightarrow0,
$$

and intersecting these decreasing tail-unions proves the claim.

The second [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) states that independent events with $\sum_n\mathbb P(A_n)=\infty$ satisfy $\mathbb P(\limsup A_n)=1$. For each fixed $N$,

$$
\mathbb P\!\left(\bigcap_{n=N}^M A_n^c\right)=\prod_{n=N}^M(1-\mathbb P(A_n))\le\exp\!\left(-\sum_{n=N}^M\mathbb P(A_n)\right)\longrightarrow0.
$$

Thus the probability that no event occurs after $N$ is zero; take the countable union over $N$ to exclude finitely many occurrences.

**As printed, the requested real logarithm is undefined:** independent [Cauchy random variables](../../../../../cauchy-random-variable.md) are negative with probability $1/2$, and the second [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md) shows that this happens infinitely often almost surely. There is therefore no real-valued sequence $\log X_n/\log n$ as stated. The natural corrected expression uses $\log|X_n|$ (or takes the limsup only over indices with $X_n>0$).

For the absolute-value interpretation,

$$
\mathbb P(|X_n|>t)=1-\frac2\pi\arctan t\sim\frac2{\pi t}\quad(t\to\infty).
$$

For every $q>1$ the events $|X_n|>n^q$ are summable and hence occur only finitely often; for $0<q\le1$ they are independent with divergent probability sum and occur infinitely often. Applying the two [Borel-Cantelli lemmas](../../../../../borel-cantelli-lemmas.md) to a countable sequence of $q$ approaching one from above and below gives

$$
\boxed{\limsup_{n\to\infty}\frac{\log|X_n|}{\log n}=1\quad\text{almost surely}.}
$$

The one-sided tail $\mathbb P(X_n>t)\sim1/(\pi t)$ gives the same constant $1$ for the positive-subsequence interpretation. It does not repair the undefined logarithms at the remaining indices unless that interpretation is explicitly adopted.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

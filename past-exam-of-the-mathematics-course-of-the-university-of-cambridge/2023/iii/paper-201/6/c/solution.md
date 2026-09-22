<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start Brownian motions at arbitrary $x,y\in\mathbb R^d$. Use the successive meeting times from part b, but after coordinate $i$ meets, drive that coordinate of the second process with the first process's increments forever. The [Strong Markov property](../../../../../../strong-markov-property.md) shows that each marginal remains a $d$-dimensional Brownian motion. By part b every coordinate is eventually locked, so the resulting [coordinatewise coalescing coupling of Brownian motions](../../../../../../coordinatewise-coalescing-coupling-of-brownian-motions.md) has an almost surely finite coalescence time $T$.

Because $f$ is bounded and harmonic, [Dynkin formula for Brownian motion](../../../../../../dynkin-formula-for-brownian-motion.md) shows that $f(B_t^x)$ and $f(B_t^y)$ are bounded [martingales](../../../../../../martingale-split.md). Therefore

$$
\begin{aligned}
|f(x)-f(y)|
&=\left|\mathbb E[f(B_t^x)-f(B_t^y)]\right|\\
&\leq2\|f\|_\infty\mathbb P(T>t).
\end{aligned}
$$

Since $T<\infty$ almost surely, the right side tends to zero. Thus $f(x)=f(y)$ for all $x,y$, proving the [Brownian coupling proof of the harmonic Liouville theorem](../../../../../../brownian-coupling-proof-of-the-harmonic-liouville-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

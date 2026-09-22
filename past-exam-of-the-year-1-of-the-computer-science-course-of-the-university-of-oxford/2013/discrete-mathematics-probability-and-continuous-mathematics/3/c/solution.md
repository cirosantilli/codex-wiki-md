<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For finite [sets](../../../../../set-split.md), the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\boxed{\left|\bigcup_{i=1}^n A_i\right|=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

An element present in $r$ of the [sets](../../../../../set-split.md) is counted $\sum_{k=1}^r(-1)^{k+1}\binom rk=1$ times, which explains the alternating corrections.

There are $\lfloor999/d\rfloor$ positive [integers](../../../../../integer-split.md) strictly below $1000$ divisible by $d$. For the divisors $2,5,7$, the single counts are $499,199,142$. Their pairwise [intersections](../../../../../set-intersection.md) correspond to divisibility by $10,14,35$, giving $99,71,28$. The triple [intersection](../../../../../set-intersection.md) has $\lfloor999/70\rfloor=14$ elements. Therefore

$$
\boxed{499+199+142-99-71-28+14=656.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

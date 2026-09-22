<h1 id="24j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $M=\|f\|_\infty>0$ and $M_0=\mu(E)$. There is a positive-measure set on which $|f|>M/2$, so $M_0>0$ and each $M_n$ is positive; boundedness and finite measure make each finite. For $n\geq1$, apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) to $|f|^{(n-1)/2}$ and $|f|^{(n+1)/2}$ to get

$$
\boxed{M_n^2\leq M_{n-1}M_{n+1}.}
$$

Therefore the positive ratios $r_n=M_{n+1}/M_n$ are nondecreasing. Telescoping gives $M_n/M_0=r_0\cdots r_{n-1}\leq r_n^n$, while $|f|^{n+1}\leq M|f|^n$ almost everywhere gives $r_n\leq M$. Hence

$$
\boxed{\mu(E)^{-1/n}\|f\|_n\leq\frac{M_{n+1}}{M_n}\leq M.}
$$

For $0<\varepsilon<M$, the set $A_\varepsilon=\{|f|>M-\varepsilon\}$ has positive measure by the definition of [essential supremum](../../../../../../essential-supremum.md). Thus $\|f\|_n\geq(M-\varepsilon)\mu(A_\varepsilon)^{1/n}$, whereas $\|f\|_n\leq M\mu(E)^{1/n}$. Letting $n\to\infty$ and then $\varepsilon\downarrow0$ shows $\mu(E)^{-1/n}\|f\|_n\to M$. The preceding squeeze yields **$M_{n+1}/M_n\to\|f\|_\infty$**. This proves the ratio limit rather than assuming it from the moment-root limit.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24J](../../24j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

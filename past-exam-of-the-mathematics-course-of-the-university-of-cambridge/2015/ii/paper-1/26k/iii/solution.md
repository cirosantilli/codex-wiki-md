<h1 id="26k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the natural urn [filtration](../../../../../../filtration-probability-theory.md). At stage $n$, put $s=X_n+Y_n=n+2$ and $d=X_n-Y_n$. The difference becomes $d-1$ with probability $X_n/s$ and $d+1$ with probability $Y_n/s$. Hence its conditional next mean is $d+(Y_n-X_n)/s=d(1-1/s)$. Since the next total is $s+1$,

$$
E[M_{n+1}\mid\mathcal F_n]=s\,d(1-1/s)=d(s-1)=M_n.
$$

Adaptedness is immediate, and every $M_n$ is bounded by a deterministic finite number, so integrable. This proves the [martingale](../../../../../../martingale-split.md) property.

Nevertheless **it does not converge to a finite limit on any sample path**. The increments are $d+s$ or $d-s$, because $M_{n+1}=s(d\pm1)$ and $M_n=(s-1)d$. Both colours remain present, so $|d|\leq s-2$ and $|M_{n+1}-M_n|\geq2$. Convergence of a real sequence would force its increments to tend to zero. There is therefore no almost-sure finite convergence, illustrating why the boundedness condition in the preceding part matters.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [26K](../../26k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

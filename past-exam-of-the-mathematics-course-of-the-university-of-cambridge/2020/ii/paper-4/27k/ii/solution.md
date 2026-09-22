<h1 id="27k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $N$ be the number of visits to the server made by one customer. Then $N$ has the [geometric distribution](../../../../../../geometric-distribution.md) with success parameter $\delta$, and its service periods $E_1,E_2,\ldots$ are independent exponential random variables of rate $\mu$. For $s\geq0$, the [Laplace transform](../../../../../../laplace-transform.md) of the total service time $T=E_1+\cdots+E_N$ is

$$
\mathbb E e^{-sT}
=\sum_{k\geq1}\delta(1-\delta)^{k-1}\left(\frac\mu{\mu+s}\right)^k
=\frac{\delta\mu}{s+\delta\mu}.
$$

Thus

$$
\boxed{T\sim\operatorname{Exp}(\delta\mu)}.
$$

At each service completion, a successful departure reduces the queue length by one and occurs at rate $\delta\mu$ while the queue is nonempty; feedback completions leave its length unchanged. The queue-length process is therefore the [birth-death process](../../../../../../birth-death-process.md) of an ordinary $M/M/1$ queue with service rate $\delta\mu$. It is positive recurrent exactly when $\lambda<\delta\mu$, and then, with $\rho=\lambda/(\delta\mu)$,

$$
\boxed{\pi_n=(1-\rho)\rho^n,\qquad n\geq0}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="27j/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here $b_n=\lambda2^{-n}$, so detailed balance gives

$$
\frac{\pi_{n+1}}{\pi_n}=\rho2^{-n}.
$$

Consequently

$$
\pi_n=\pi_0\rho^n2^{-n(n-1)/2},
\qquad
\boxed{\pi_0=
\left(\sum_{n=0}^{\infty}\rho^n2^{-n(n-1)/2}\right)^{-1}}.
$$

The series converges for every $\rho>0$, so this defines the unique invariant distribution.

By the [PASTA property](../../../../../../../poisson-arrivals-see-time-averages.md), an arrival joins with probability $\sum_{n\geq0}\pi_np(n)$. In equilibrium the accepted-arrival rate must also equal the departure rate. Departures occur at rate $\mu$ precisely when the queue is nonempty, hence

$$
\lambda\sum_{n\geq0}\pi_np(n)=\mu(1-\pi_0).
$$

The required joining probability is therefore

$$
\boxed{\sum_{n\geq0}\pi_np(n)=\frac{\mu(1-\pi_0)}{\lambda}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [27J](../../../27j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

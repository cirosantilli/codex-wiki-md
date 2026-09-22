<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In Kendall notation, the first two letters $M$ mean [Poisson arrivals](../../../../../../poisson-process.md) and [exponential service times](../../../../../../exponential-distribution.md). An [M/M/1 queue](../../../../../../m-m-1-queue.md) has arrival rate $\lambda$, one server of rate $\mu$, and queue-length transitions

$$
n\to n+1\text{ at rate }\lambda,
\qquad
n\to n-1\text{ at rate }\mu\quad(n\geq1).
$$

It has a [stationary distribution of an M-M-1 queue](../../../../../../stationary-distribution-of-an-m-m-1-queue.md) exactly when

$$
\rho:=\frac\lambda\mu<1,
$$

and then

$$
\boxed{\pi_n=(1-\rho)\rho^n,
\qquad n\geq0.}
$$

An [M-M-infinity queue](../../../../../../m-m-%E2%88%9E-queue.md) has infinitely many servers, so every customer begins service immediately. Its occupancy transitions are

$$
n\to n+1\text{ at rate }\lambda,
\qquad
n\to n-1\text{ at rate }n\mu.
$$

The [detailed balance for a birth-death process](../../../../../../detailed-balance-for-a-birth-death-process.md) equations give

$$
\pi_{n+1}=\pi_n\frac{\lambda}{(n+1)\mu}.
$$

Thus for every $\lambda,\mu>0$ the [stationary distribution of an M-M-infinity queue](../../../../../../stationary-distribution-of-an-m-m-infinity-queue.md) exists and is

$$
\boxed{\pi_n=e^{-\rho}\frac{\rho^n}{n!},
\qquad \rho=\frac\lambda\mu,}
$$

the [Poisson distribution](../../../../../../poisson-distribution.md) of mean $\rho$. The [Burke theorem for an M-M-infinity queue](../../../../../../burke-theorem-for-an-m-m-infinity-queue.md) states that in this stationary regime the departure process is a [Poisson process](../../../../../../poisson-process.md) of rate $\lambda$; equivalently, time reversal turns departures into arrivals. The past departure process is also independent of the number in the system at the observation time.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

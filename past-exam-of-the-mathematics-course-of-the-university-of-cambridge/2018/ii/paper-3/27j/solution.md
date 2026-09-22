<h1 id="27j/solution">Solution</h1>

↑ **Parent:** [27J](../27j.md)

Immediately after departure $n$, either $Q_n>0$ and one of those customers starts the next service, or $Q_n=0$ and the next arrival both initiates service and is not counted among those waiting after it. During that service $A_n$ further customers arrive. Thus the [embedded departure chain of an M-G-1 queue](../../../../../embedded-departure-chain-of-an-m-g-1-queue.md) obeys

$$
\boxed{Q_{n+1}=A_n+Q_n-h(Q_n),\qquad h(x)=\min\{1,x\}.}
$$

Conditional on the next service time $S_{n+1}=s$, the [Poisson process](../../../../../poisson-process.md) property gives

$$
A_n\mid S_{n+1}=s\sim\operatorname{Poisson}(\lambda s).
$$

The [law of total expectation](../../../../../law-of-total-expectation.md) and [law of total variance](../../../../../law-of-total-variance.md) therefore give

$$
\boxed{\mathbb EA_n=\lambda\mathbb ES=\rho,}
$$

and

$$
\boxed{\mathbb EA_n^2
=\mathbb E[\lambda S+(\lambda S)^2]
=\rho+\lambda^2\mathbb ES^2.}
$$

In equilibrium let $Q$ have the common distribution of $Q_n,Q_{n+1}$ and put $H=\mathbf1_{\{Q>0\}}=h(Q)$. The fresh pair $(A_n,S_{n+1})$ is independent of $Q_n$. Taking expectations in the recursion gives

$$
0=\rho-\mathbb EH,
\qquad\text{so}\qquad
\mathbb P(Q>0)=\rho.
$$

Because $QH=Q$ and $H^2=H$, stationarity of the second moment gives

$$
\begin{aligned}
0
&=\mathbb E[(Q-H+A)^2-Q^2]\\
&=-2\mathbb EQ+\rho
+2\rho(\mathbb EQ-\rho)
+\rho+\lambda^2\mathbb ES^2.
\end{aligned}
$$

Solving,

$$
\boxed{\mathbb EQ
=\rho+\frac{\lambda^2\mathbb ES^2}{2(1-\rho)}.}
$$

In stationarity, level crossing together with [Poisson arrivals see time averages](../../../../../poisson-arrivals-see-time-averages.md) identifies this as the mean number $L$ in the shop. The [Little law](../../../../../little-s-law.md) gives $L=\lambda(W_q+\mathbb ES)$, where $W_q$ is waiting time before service. Since $\rho=\lambda\mathbb ES$,

$$
\boxed{W_q=\frac{\lambda\mathbb ES^2}{2(1-\rho)}.}
$$

This is the [Pollaczek-Khinchine mean formula](../../../../../pollaczek-khinchine-mean-formula.md).

## ↑ Ancestors (10)

1. [27J](../27j.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The displayed equation has nominal orders $p=1,q=2$, with

$$
\Phi(z)=1-0.5z,\qquad
\Theta(z)=1-1.4z+0.45z^2=(1-0.5z)(1-0.9z).
$$

The AR root is $2$, and the MA roots are $2$ and $10/9$, all strictly outside the unit disc. Thus its stationary solution is causal and invertible. There is also [common factor cancellation in an ARMA model](../../../../../../common-factor-cancellation-in-an-arma-model.md): the convergent inverse of $1-0.5B$ cancels the shared factor, giving

$$
\boxed{x_t=w_t-0.9w_{t-1}.}
$$

Consequently **the displayed representation is ARMA(1,2), but its minimal order is ARMA(0,1)**. This also follows without formal operator cancellation: the difference between any solution and the right-hand side satisfies $d_t=0.5d_{t-1}$. A stationary finite-variance difference must have zero [variance](../../../../../../variance-split.md), since stationarity would give $\operatorname{Var}(d_t)=0.25\operatorname{Var}(d_t)$; its constant mean must also vanish. A transient chosen by an arbitrary initial condition is not the stationary process whose ACF is requested.

For this [moving-average model](../../../../../../moving-average-model.md), [independence](../../../../../../independent-random-variables.md) of the noise gives

$$
\gamma(0)=(1+0.9^2)\sigma_w^2=1.81\sigma_w^2,\qquad
\gamma(1)=\gamma(-1)=-0.9\sigma_w^2,
$$

while $\gamma(h)=0$ for $|h|\ge2$, since the two noise sets are disjoint. Therefore its [autocorrelation function](../../../../../../autocorrelation.md) is

$$
\boxed{\rho(h)=\begin{cases}
1,&h=0,\\
-90/181,&|h|=1,\\
0,&|h|\ge2.
\end{cases}}
$$

The reduced moving-average inverse is $w_t=\sum_{j\ge0}0.9^jx_{t-j}$, whose coefficients are absolutely summable, confirming invertibility directly.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

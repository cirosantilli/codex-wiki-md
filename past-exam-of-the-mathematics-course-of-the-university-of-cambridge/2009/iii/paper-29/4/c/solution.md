<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $k(x,t)=h_x(x,t)/h(x,t)=\partial_x\log h(x,t)$. Positivity and smoothness of $h$ make $k$ continuous and bounded on compact space-time sets. Brownian paths remain in compact spatial sets on each finite horizon, so $\int_0^Tk(X_s,s)^2ds<\infty$ almost surely for every $T$. Thus

$$
M_t=\int_0^tk(X_s,s)dX_s
$$

is a well-defined [continuous local martingale](../../../../../../continuous-local-martingale.md) with $M_0=0$. The backward heat equation from part (b) removes the drift in Itô's formula and yields

$$
dZ_t=h_x(X_t,t)dX_t=Z_t\,dM_t.
$$

By the allowed fact $Z_0=1$ and the uniqueness in part (a),

$$
\boxed{Z_t=\mathcal E(M)_t=\exp\!\left(\int_0^tk(X_s,s)dX_s-\frac12\int_0^tk(X_s,s)^2ds\right).}
$$

The finite-horizon form of the [Girsanov theorem](../../../../../../girsanov-theorem.md) used here says: if $M_0=0$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) and its stochastic exponential $Z$ is a strictly positive true [martingale](../../../../../../martingale-split.md) of mean one on $[0,T]$, then under $d\mathbb Q|_{\mathcal F_T}=Z_Td\mathbb P|_{\mathcal F_T}$ every continuous $\mathbb P$-local [martingale](../../../../../../martingale-split.md) $N$ becomes the $\mathbb Q$-local [martingale](../../../../../../martingale-split.md) $N-[N,M]$. [Quadratic variation](../../../../../../quadratic-variation.md) is unchanged by this locally equivalent change of measure.

All the assumptions hold. The integrand defining $M$ is locally square integrable as checked above; $Z$ is strictly positive; and it is already a true [martingale](../../../../../../martingale-split.md) because it is the density process. On each finite horizon $Z_t=\mathbb E[Z_T\mid\mathcal F_t]$, so it is [uniformly integrable](../../../../../../uniform-integrability.md) on that horizon. There is no need to establish a separate Novikov condition, nor to assume equivalence on the infinite-time sigma-algebra.

Take $N=X$. Its covariation with $M$ is $[X,M]_t=\int_0^tk(X_s,s)ds$. Hence $B_t=X_t-\int_0^tk(X_s,s)ds$ is a continuous $\mathbb Q$-local [martingale](../../../../../../martingale-split.md) starting at zero with $[B]_t=t$. The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) makes it Brownian under $\mathbb Q$. Since this argument holds on every finite horizon for the same process $B$,

$$
\boxed{X_t=B_t+\int_0^t\frac{h_x(X_s,s)}{h(X_s,s)}ds,\qquad B\text{ is Brownian motion under }\mathbb Q.}
$$

This is the [Brownian change of measure by a positive space-time harmonic function](../../../../../../brownian-change-of-measure-by-a-positive-space-time-harmonic-function.md), a [Doob h-transform](../../../../../../doob-h-transform.md) with drift $\partial_x\log h$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

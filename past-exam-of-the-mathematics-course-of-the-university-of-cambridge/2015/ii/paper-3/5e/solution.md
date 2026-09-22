<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

There are $kx_n$ seeds and their germinating proportion is $e^{-\gamma x_n}$, giving the [survival-augmented Ricker map](../../../../../survival-augmented-ricker-map.md) with zero survival. A positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) satisfies $e^{-\gamma x_*}=1/k$, so

$$
x_*=\frac{\log k}{\gamma},\qquad F'(x_*)=1-\log k.
$$

It exists when $k>1$ and is strictly [linearly stable](../../../../../linear-stability.md) when $|1-\log k|<1$. Thus **the usual strict linear-stability interval is** $\boxed{1<k<e^2}$.

With winter survival, surviving adults and new plants add:

$$
x_{n+1}=sx_n+kx_ne^{-\gamma x_n},\qquad x_* =\frac1\gamma\log\frac{k}{1-s}.
$$

Writing $L=\log[k/(1-s)]$, the [linearization of a dynamical system](../../../../../linearization-of-a-dynamical-system.md) has multiplier $1-(1-s)L$. Hence **the strict linear-stability interval becomes**

$$
\boxed{1-s<k<(1-s)\exp\!\left(\frac2{1-s}\right).}
$$

Its lower endpoint is less than $1$. Its upper endpoint exceeds $e^2$: for $t=1-s\in(0,1)$, $\log t+2/t$ is decreasing in $t$ and equals $2$ at $t=1$.

The [nonlinear stability at the Ricker flip threshold](../../../../../nonlinear-stability-at-the-ricker-flip-threshold.md) needs a separate check. The upper endpoints have multiplier $-1$, so the strict linear test alone does not decide stability there. They are in fact locally [asymptotically stable](../../../../../asymptotic-stability.md), with algebraic rather than geometric convergence. To see this, put $u=\gamma(x-x_*)$ at $L=2/(1-s)$. The local map is

$$
u\longmapsto-u+su^2+\left(\frac{1-s}{2}-\frac13\right)u^3+O(u^4),
$$

and its second iterate is $u-2(s^2-s/2+1/6)u^3+O(u^4)$. The cubic coefficient in parentheses is positive for every $s\in[0,1)$. Thus, if “stable” includes nonlinear endpoint stability, the upper inequalities can be replaced by $\leq$; the lower endpoints have no positive equilibrium.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

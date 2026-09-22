<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Korovkin theorem](../../../../../korovkin-theorem.md) states that if [positive linear operators on continuous functions](../../../../../positive-linear-operator-on-continuous-functions.md) $L_n:C[0,1]\to C[0,1]$ satisfy

$$
\|L_ne_j-e_j\|_\infty\longrightarrow0,\qquad e_j(t)=t^j,\quad j=0,1,2,
$$

then $\|L_nf-f\|_\infty\to0$ for every real [continuous function](../../../../../continuous-function.md) $f$.

Let $r=k-1\ge2$ and $h_n=|\Delta_n|$. For the [B-splines](../../../../../b-spline.md) in this question, $N_{i,n}\ge0$ and their sum is one on the basic interval. Thus the [Schoenberg spline operator](../../../../../schoenberg-spline-operator.md) $V_n$ is linear and positive. To verify the three test [functions](../../../../../function-split.md), suppress the index $n$ and write the [Marsden identity](../../../../../marsden-identity.md) with $\omega_i(x)=\prod_{j=1}^r(x-t_{i+j})$. Comparing the coefficients of $x^r,x^{r-1},x^{r-2}$ gives the [monomial B-spline coefficients](../../../../../monomial-b-spline-coefficients.md)

$$
1=\sum_iN_i(t),\qquad
 t=\sum_i\xi_iN_i(t),\qquad
 t^2=\sum_iq_iN_i(t),
$$

where

$$
\xi_i=\frac1r\sum_{j=1}^rt_{i+j},\qquad
q_i=\frac1{\binom r2}\sum_{1\le j<\ell\le r}t_{i+j}t_{i+\ell}.
$$

The first coefficient is the partition of unity; the second is the [Greville abscissa](../../../../../greville-abscissa.md). Every internal knot and the sample point $\tau_i$ lie in $[t_i,t_{i+k}]$, of width at most $kh_n$. Consequently $|\tau_i-\xi_i|\le kh_n$. Since all these numbers lie in $[0,1]$, for any two internal knots $u,v$ we also have

$$
|\tau_i^2-uv|\le|\tau_i|\,|\tau_i-u|+|u|\,|\tau_i-v|\le2kh_n.
$$

Averaging gives $|\tau_i^2-q_i|\le2kh_n$. Nonnegative weights of sum one now yield

$$
\|V_n1-1\|_\infty=0,\qquad
\|V_ne_1-e_1\|_\infty\le kh_n,\qquad
\|V_ne_2-e_2\|_\infty\le2kh_n.
$$

Here the [spline](../../../../../spline-mathematics.md) order $k$ is fixed, so all three errors tend to zero. The [Korovkin theorem](../../../../../korovkin-theorem.md) therefore proves

$$
\boxed{\|V_nf-f\|_\infty\longrightarrow0\quad\text{for every }f\in C[0,1].}
$$

No special selection such as the [Greville abscissae](../../../../../greville-abscissa.md) is required for the sample points. In fact the [local-support error bound for a Schoenberg spline operator](../../../../../local-support-error-bound-for-a-schoenberg-spline-operator.md) also gives $\|V_nf-f\|_\infty\le\omega(f,kh_n)$. Under the usual continuous-spline convention the operators have the codomain required by the stated theorem. If the permissive knot notation is taken to allow full interior multiplicities and hence discontinuous [splines](../../../../../spline-mathematics.md), the same conclusion in the uniform [norm](../../../../../norm.md) still follows from this direct bound, although each approximant need not then be continuous.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

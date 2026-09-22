<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $N_{i,d}$ for the partition-of-unity-normalized degree-$d$ [B-spline](../../../../../b-spline.md), supported on $[t_i,t_{i+d+1}]$. Assume $d\ge1$. First take distinct knots; endpoint repetitions will be interpreted as confluent limits. For fixed parameter $t$, let $f_t(\tau)=(\tau-t)_+^d$, and form

$$
N_{i,d}(t)=(t_{i+d+1}-t_i)[t_i,\ldots,t_{i+d+1}]f_t,
$$

where the brackets denote a [divided difference](../../../../../divided-difference.md) in the knot variable $\tau$. This representation follows from the defining properties, rather than assuming a derivative recurrence. If $t<t_i$, $f_t$ is a degree-$d$ polynomial in all its knot arguments and its order-$(d+1)$ [divided difference](../../../../../divided-difference.md) is zero. If $t>t_{i+d+1}$, every truncated-power term is zero. Between knots it is a degree-$d$ polynomial with $d-1$ continuous [derivatives](../../../../../derivative.md). Those support and smoothness conditions determine a one-dimensional spline space: there are $d+1$ spans, the continuity conditions leave $2d+1$ coefficients, and vanishing through order $d-1$ at both support ends imposes $2d$ conditions.

The remaining scalar is fixed by the prescribed integral. Put $a=t_i$, $b=t_{i+d+1}$. Integrating the truncated power first gives

$$
\int_a^b(\tau-t)_+^d\,dt=\frac{(\tau-a)^{d+1}}{d+1}\quad(a\le\tau\le b).
$$

The order-$(d+1)$ [divided difference](../../../../../divided-difference.md) of this polynomial is its leading coefficient $1/(d+1)$, so the proposed $N_{i,d}$ has integral $(b-a)/(d+1)$, exactly the specified normalization.

Now differentiate with respect to $t$ and apply the final recursion for a [divided difference](../../../../../divided-difference.md):

$$
\begin{aligned}
N_{i,d}'(t)
&=-d(t_{i+d+1}-t_i)[t_i,\ldots,t_{i+d+1}](\tau-t)_+^{d-1}\\
&=d[t_i,\ldots,t_{i+d}](\tau-t)_+^{d-1}
-d[t_{i+1},\ldots,t_{i+d+1}](\tau-t)_+^{d-1}.
\end{aligned}
$$

In terms of normalized lower-degree [B-splines](../../../../../b-spline.md), this is the [B-spline differentiation formula](../../../../../b-spline-differentiation-formula.md)

$$
\boxed{N_{i,d}'=\frac d{t_{i+d}-t_i}N_{i,d-1}
-\frac d{t_{i+d+1}-t_{i+1}}N_{i+1,d-1}.}
$$

A zero denominator corresponds to a collapsed-support basis term and contributes zero. Repeated knots follow by coalescing distinct knots; at knots where the classical derivative is discontinuous, read the formula on each open span or one-sided. The stated maximal interior continuity corresponds to simple interior knots, while the clamped endpoint repetitions do not affect the interior argument.

Let the control-point abscissae be the [Greville abscissae](../../../../../greville-abscissa.md)

$$
\xi_i=\frac1d\sum_{r=1}^dt_{i+r},\qquad X(t)=\sum_{i=0}^n\xi_iN_{i,d}(t).
$$

Collect the coefficient of $N_{i,d-1}$ after differentiating:

$$
X'(t)=\sum_{i=1}^n\frac{d(\xi_i-\xi_{i-1})}{t_{i+d}-t_i}N_{i,d-1}(t).
$$

The difference of the two consecutive knot averages telescopes to

$$
\xi_i-\xi_{i-1}=\frac{t_{i+d}-t_i}{d},
$$

so every noncollapsed coefficient is one. The lower-degree basis on the endpoint-trimmed knot vector has [partition of unity](../../../../../partition-of-unity.md); equivalently the outer lower-degree basis functions on the original vector have collapsed support. Therefore $X'(t)=1$ on the parameter interval. With $d+1$ repeated left endpoint knots at $a$, the clamped basis has $N_{0,d}(a)=1$, all other values zero, and $\xi_0=a$. Thus $X(a)=a$ fixes the constant of integration. Continuity and endpoint limits now give

$$
\boxed{X(t)=t\quad\text{throughout the basic parameter interval}.}
$$

This is [linear precision at Greville abscissae](../../../../../linear-precision-at-greville-abscissae.md). It requires neither equal knot spacing nor a restriction on the other control-point coordinates; those determine the remaining coordinates of the [parametric curve](../../../../../parametric-curve.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

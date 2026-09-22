<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $t$ and let $F_t(u)=(u-t)_+^{k-1}$. Initially assume distinct [spline knots](../../../../../../spline-knot.md), so the ordinary [polynomial interpolation](../../../../../../polynomial-interpolation.md) definitions are unambiguous. The two interpolants $\ell_i(\cdot,t)$ and $\ell_{i+1}(\cdot,t)$ agree with $F_t$ at their $k-1$ shared nodes $t_{i+1},\ldots,t_{i+k-1}$. Their difference has degree at most $k-1$ and all these roots, hence

$$
\ell_{i+1}(x,t)-\ell_i(x,t)=c_i(t)\prod_{r=1}^{k-1}(x-t_{i+r})=c_i(t)\omega_i(x).
$$

For $k=1$ the product is empty and the same statement concerns constants. The [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md) of an interpolating polynomial is its highest-order [divided difference](../../../../../../divided-difference.md), so the [divided difference](../../../../../../divided-difference.md) recurrence gives

$$
\begin{aligned}
c_i(t)&=[t_{i+1},\ldots,t_{i+k}]F_t-[t_i,\ldots,t_{i+k-1}]F_t\\
&=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]F_t=N_i(t).
\end{aligned}
$$

This proves [Lee's formula](../../../../../../lee-interpolation-identity.md):

$$
\boxed{\ell_{i+1}(x,t)-\ell_i(x,t)=\omega_i(x)N_i(t).}
$$

Summing over $i$ telescopes to $\ell_{n+1}(x,t)-\ell_1(x,t)$. If $t_k<t<t_{n+1}$, the first interpolation nodes $t_1,\ldots,t_k$ are all smaller than $t$, so their truncated-power data vanish and $\ell_1=0$. The last nodes $t_{n+1},\ldots,t_{n+k}$ are larger than $t$, so their data are values of the polynomial $(u-t)^{k-1}$ and uniqueness gives $\ell_{n+1}(x,t)=(x-t)^{k-1}$. Thus **the telescoped identity is**

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),\qquad t_k<t<t_{n+1},}
$$

the [Marsden identity](../../../../../../marsden-identity.md), valid for every real $x$.

If repeated [spline knots](../../../../../../spline-knot.md) are allowed, ordinary value interpolation at repeated nodes does not specify $\ell_i$ uniquely. The standard extension uses confluent [divided differences](../../../../../../divided-difference.md) and [Hermite interpolation](../../../../../../hermite-interpolation.md), or limits of distinct knots: the same polynomial identity then persists wherever these quantities are defined. At a maximally repeated knot where the truncated power lacks the required derivative, the appropriate one-sided spline convention must be fixed; an unspecified classical derivative is not part of the proof. For distinct knots, the printed identity requires no such qualification.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

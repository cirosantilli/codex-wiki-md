<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original PDF has $u_m^{n+1}$ on the left of the update; the converted TeX omits its $+1$. Use the [Forward Euler method](../../../../../../euler-method.md) with $k=\Delta t\geq0$ and $\mu=k/h_x^2$. The [explicit time stepping for bounded reaction diffusion](../../../../../../explicit-time-stepping-for-bounded-reaction-diffusion.md) update [matrix](../../../../../../matrix.md) is

$$
 E_h=H_h+kV_h,\qquad H_h=I+kD_h.
$$

When $0\leq\mu\leq1/2$, the heat update $H_h$ has nonnegative stencil weights $\mu,1-2\mu,\mu$ and row sums at most one. Hence its induced maximum [operator norm](../../../../../../operator-norm.md) is at most one. It is also a [symmetric matrix](../../../../../../symmetric-matrix.md) with [eigenvalues](../../../../../../eigenvalue.md)

$$
 1-4\mu\sin^2\frac{j\pi}{2(M+1)},\qquad 1\leq j\leq M,
$$

all in $[-1,1]$, so its discrete [L2 norm](../../../../../../l2-norm.md) operator bound is at most one too. Let $A_*=\max(|a_0|,|a_+|)$. In either of these [norms](../../../../../../norm.md),

$$
\|E_h\|\leq\|H_h\|+k\|V_h\|\leq1+kA_*.
$$

Iteration gives the mesh-uniform [stability](../../../../../../stability-of-a-numerical-method.md) estimate

$$
\boxed{\|u^n\|\leq(1+kA_*)^n\|u^0\|\leq e^{A_*nk}\|u^0\|,
\qquad nk\leq T.}
$$

The same estimate applies to differences of solutions. Adding a per-step defect $kr^n$ gives $\|e^n\|\leq e^{A_*T}(\|e^0\|+k\sum_{j<n}\|r^j\|)$.

This proof only requires $\mu\leq1/2$ and bounded reaction coefficients. It does not assume the full update $E_h$ is nonnegative: a negative $a_m$ can make its middle stencil weight negative when $\mu=1/2$. Nor does it claim contractivity or an all-time bound for every coefficient. The required [stability](../../../../../../stability-of-a-numerical-method.md) is a bound uniform in the discretization on fixed finite intervals.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

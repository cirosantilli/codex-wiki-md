<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f_i=f(ih)$ and $g_i=g(ih)$, and define the scaled [forward difference operator](../../../../forward-difference-operator.md), [backward difference operator](../../../../backward-difference-operator.md) and [second-order central difference](../../../../second-order-central-difference.md) by

$$
D_x^+W_i=\frac{W_{i+1}-W_i}{h},\qquad D_x^-W_i=\frac{W_i-W_{i-1}}h,\qquad
D_x^+D_x^-W_i=\frac{W_{i+1}-2W_i+W_{i-1}}{h^2}.
$$

The two [finite difference methods](../../../../finite-difference-method.md) are the nonlinear systems

$$
\boxed{-D_x^+D_x^-U_i+U_i+U_i^3=f_i,\qquad -D_x^+D_x^-V_i+V_i+V_i^3=g_i,\quad 1\leq i\leq N-1,}
$$

with the prescribed [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md) $U_0=V_0=A$ and $U_N=V_N=B$. These equations determine the interior nodal values.

For clarity distinguish the interior and edge [inner products](../../../../inner-product-split.md) and their [norms](../../../../norm.md):

$$
(P,Q)_h=h\sum_{i=1}^{N-1}P_iQ_i,\quad
(P,Q]_{h}=h\sum_{i=1}^NP_iQ_i,\quad
\|P\|_h^2=(P,P)_h,\quad
\|P]\!\|_h^2=(P,P]_{h}.
$$

The bracketed [norm](../../../../norm.md) includes the last edge $i=N$. Let $W=U-V$, so $W_0=W_N=0$, and put $q_i=D_x^-W_i$ for $1\leq i\leq N$. Direct telescoping gives [discrete summation by parts](../../../../discrete-summation-by-parts.md):

$$
(-D_x^+D_x^-W,W)_h
=-\sum_{i=1}^{N-1}(q_{i+1}-q_i)W_i
=\sum_{i=1}^Nq_i(W_i-W_{i-1})
=h\sum_{i=1}^Nq_i^2.
$$

Subtract the two nonlinear systems, multiply each equation by $hW_i$ and sum. The resulting discrete [energy identity](../../../../energy-identity.md) is

$$
\|D_x^-W]\!\|_h^2+\|W\|_h^2+h\sum_{i=1}^{N-1}(U_i^3-V_i^3)W_i=(f-g,W)_h.
$$

The nonlinear summands are nonnegative by the factorization in (a). Using [Young's inequality for products](../../../../young-s-inequality-for-products.md) at every node gives

$$
\boxed{\|D_x^-U-D_x^-V]\!\|_h^2+\frac12\|U-V\|_h^2\leq\frac12\|f-g\|_h^2.}
$$

This also proves [uniqueness](../../../../uniqueness.md) of each discrete solution. Existence can be seen by minimizing, with the endpoints fixed, the [strictly convex](../../../../strictly-convex-function.md) [energy functional](../../../../energy-functional.md)

$$
J_f(W)=\frac h2\sum_{i=1}^N(D_x^-W_i)^2+h\sum_{i=1}^{N-1}\left(\frac{W_i^2}2+\frac{W_i^4}4-f_iW_i\right).
$$

It is a [coercive function](../../../../coercive-function.md) of its finitely many interior values, so it attains a minimum. Its first [derivatives](../../../../derivative.md) are $h(-D_x^+D_x^-W_i+W_i+W_i^3-f_i)$; thus its [minimizer](../../../../global-minimizer.md) solves the scheme. The same argument applies to $g$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $f$ be continuous in its first variable and uniformly [Lipschitz continuous](../../../../lipschitz-continuity.md) in its second variable, with constant $L\geq0$. Retain the finite-interval smoothness assumptions and the bound $\|\tau_n\|\leq Kh^2$ from the preceding subpart. We first establish solvability of each implicit step. For a proposed starting state $u$, the map

$$
G_u(v)=u+h f\left(x_n+\frac h2,\frac{u+v}2\right)
$$

has [Lipschitz constant](../../../../lipschitz-constant.md) $hL/2$. If $hL/2<1$, the [contraction mapping theorem](../../../../contraction-mapping-theorem.md) on the complete state space gives a unique next state $v=\Psi_{n,h}(u)$.

To compute a useful [Lipschitz constant](../../../../lipschitz-constant.md) for the method, introduce its increment function by

$$
\Psi_{n,h}(u)=u+h\Phi_{n,h}(u),\qquad
\Phi_{n,h}(u)=f\left(x_n+\frac h2,u+\frac h2\Phi_{n,h}(u)\right).
$$

For two starting states $u,w$,

$$
\|\Phi_{n,h}(u)-\Phi_{n,h}(w)\|
\leq L\|u-w\|+\frac{hL}{2}
\|\Phi_{n,h}(u)-\Phi_{n,h}(w)\|.
$$

Rearranging gives the [implicit midpoint Lipschitz estimate](../../../../implicit-midpoint-lipschitz-estimate.md)

$$
\boxed{\operatorname{Lip}(\Phi_{n,h})\leq\frac{L}{1-hL/2},
\qquad
\operatorname{Lip}(\Psi_{n,h})\leq
R_h:=\frac{1+hL/2}{1-hL/2}.}
$$

Thus, for example, $hL\leq1$ gives an increment [Lipschitz constant](../../../../lipschitz-constant.md) at most $2L$, uniformly as $h\to0$.

For an explicit [global error](../../../../global-discretization-error.md) estimate, set $e_n=Y_n-y_n$. Subtract the numerical formula from the exact-value identity containing $h\tau_n$:

$$
e_{n+1}=e_n+h\left[
f\left(x_n+\frac h2,\frac{Y_n+Y_{n+1}}2\right)
-f\left(x_n+\frac h2,\frac{y_n+y_{n+1}}2\right)\right]+h\tau_n.
$$

The [Lipschitz condition](../../../../lipschitz-continuity.md) and the [triangle inequality](../../../../triangle-inequality.md) imply

$$
(1-hL/2)\|e_{n+1}\|
\leq(1+hL/2)\|e_n\|+h\|\tau_n\|,
$$

and therefore

$$
\|e_{n+1}\|\leq R_h\|e_n\|+
\frac{Kh^3}{1-hL/2}.
$$

Iterating this inequality is the elementary [discrete Gronwall inequality](../../../../discrete-gronwall-inequality.md) argument. For $L>0$, summing the [geometric series](../../../../geometric-series.md) and using $R_h-1=hL/(1-hL/2)$ gives

$$
\|e_n\|\leq R_h^n\|e_0\|+
\frac{Kh^2}{L}(R_h^n-1).
$$

For $hL\leq1$, $R_h=1+hL/(1-hL/2)\leq1+2hL\leq e^{2hL}$. If $nh\leq T$, this proves

$$
\boxed{\max_{nh\leq T}\|e_n\|
\leq e^{2LT}\|e_0\|+
\frac{K}{L}(e^{2LT}-1)h^2.}
$$

With the exact initial value, $e_0=0$, the [global error](../../../../global-discretization-error.md) is $O(h^2)$ and tends uniformly to zero on every such finite interval. If $L=0$, the recurrence instead gives $\|e_n\|\leq\|e_0\|+KTh^2$, with the same conclusion. Starting values merely converging to the exact initial value also suffice for [numerical convergence](../../../../convergence-of-a-numerical-method.md); second-order accuracy requires their errors to be $O(h^2)$. The result concerns exact implicit solves and convergence on fixed finite intervals, not uniform accuracy over an unbounded time interval.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

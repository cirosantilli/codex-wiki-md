<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Runge-Kutta method](../../../../../runge-kutta-method.md) with stage [matrix](../../../../../matrix.md) $A$, weights $b$ and [step size](../../../../../step-size.md) $h$ is

$$
Y_i=y_n+h\sum_j a_{ij}f(Y_j),\qquad y_{n+1}=y_n+h\sum_i b_i f(Y_i).
$$

Its order measures accuracy as $h\to0$, while stability concerns how errors or stiff components propagate. Linear [A-stability](../../../../../a-stability.md), strong stiff damping through [L-stability](../../../../../l-stability.md), and nonlinear [B-stability](../../../../../b-stability.md) address different questions.

For the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$, elimination of the stages gives the [stability function](../../../../../stability-function.md)

$$
R(z)=1+zb^T(I-zA)^{-1}\mathbf1,\qquad z=h\lambda.
$$

The [linear stability domain](../../../../../linear-stability-domain.md) is $\{z:|R(z)|\leq1\}$. The method is [A-stable](../../../../../a-stability.md) when it contains the closed left half-plane, and [L-stable](../../../../../l-stability.md) when it is also true that $R(z)\to0$ as $|z|\to\infty$ there. These conditions describe, respectively, stability for every non-growing scalar linear mode and damping of very rapidly decaying modes.

The [Forward Euler method](../../../../../euler-method.md) has $R(z)=1+z$, so it fails [A-stability](../../../../../a-stability.md), for example at $z=-3$. In fact no nontrivial explicit [Runge-Kutta method](../../../../../runge-kutta-method.md) is [A-stable](../../../../../a-stability.md): its [stability function](../../../../../stability-function.md) is a nonconstant [polynomial](../../../../../polynomial-split.md), which is unbounded along the negative real axis. The [Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=1/(1-z)$. For $\operatorname{Re}z\leq0$, $|1-z|\geq1$, and the function tends to zero at infinity, proving both [A-stability](../../../../../a-stability.md) and [L-stability](../../../../../l-stability.md). The [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) has $R(z)=(1+z/2)/(1-z/2)$. The identity $|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z$ proves [A-stability](../../../../../a-stability.md), but its limit $-1$ rules out [L-stability](../../../../../l-stability.md).

For nonlinear equations, a [dissipative vector field](../../../../../dissipative-vector-field.md) satisfies $\langle f(x)-f(y),x-y\rangle\leq0$. The corresponding exact solutions contract because the time derivative of their squared distance is twice that [inner product](../../../../../inner-product.md). A [B-stable](../../../../../b-stability.md) method preserves this contraction for every $h>0$, whenever its stages are well defined.

Let $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$, and $F_i=f(Y_i)-f(\widetilde Y_i)$. Expanding the update's squared [norm](../../../../../norm.md), substituting $d=D_i-h\sum_j a_{ij}F_j$, and symmetrizing the double sum proves the [Runge-Kutta contractivity identity](../../../../../runge-kutta-contractivity-identity.md)

$$
\|d_{n+1}\|^2-\|d\|^2
=2h\sum_i b_i\langle D_i,F_i\rangle-h^2\sum_{i,j}m_{ij}\langle F_i,F_j\rangle,
\quad m_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

If $b_i\geq0$ and the [matrix](../../../../../matrix.md) $M=(m_{ij})$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), the first sum is nonpositive by dissipativity. The second double sum is nonnegative: sum the [quadratic form](../../../../../quadratic-form.md) of $M$ over each coordinate of the $F_i$. Thus **[algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) implies [B-stability](../../../../../b-stability.md)**. Applied to complex scalar linear equations with the real part of the Hermitian [inner product](../../../../../inner-product.md), the same argument also implies [A-stability](../../../../../a-stability.md), where the stages are defined.

The [Backward Euler method](../../../../../backward-euler-method.md) has $b_1=a_{11}=1$, hence $M=(1)$, and is [algebraically stable](../../../../../algebraic-stability-of-a-runge-kutta-method.md). One can prove its nonlinear contraction directly: $d_{n+1}=d+h(f(y_{n+1})-f(\widetilde y_{n+1}))$ gives $\|d_{n+1}\|^2\leq\langle d,d_{n+1}\rangle\leq\|d\|\|d_{n+1}\|$. The [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) has $a_{11}=1/2$, $b_1=1$ and $M=0$, so it is [B-stable](../../../../../b-stability.md) even though it is not [L-stable](../../../../../l-stability.md).

Linear [A-stability](../../../../../a-stability.md) does not by itself imply nonlinear [B-stability](../../../../../b-stability.md). The ODE [trapezoidal rule](../../../../../trapezoidal-rule.md) has the same [stability function](../../../../../stability-function.md) as the [implicit midpoint rule](../../../../../implicit-midpoint-rule.md), but take the dissipative scalar field $f(y)=-\max(y,0)$ and $h=6$. For any positive starting value, its trapezoidal update is $y_{n+1}=y_n+3(f(y_n)+f(y_{n+1}))=-2y_n<0$. Thus two positive starting values have their distance doubled, violating [B-stability](../../../../../b-stability.md). Its [algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) [matrix](../../../../../matrix.md) also has a negative first diagonal entry. The field is globally [Lipschitz continuous](../../../../../lipschitz-continuity.md), so this is a well-defined nonlinear counterexample.

These examples distinguish accuracy, scalar stiff-mode stability, nonlinear contraction, and rapid stiff-mode damping. For implicit methods, solvability of the stage equations remains an additional requirement; a formal [stability function](../../../../../stability-function.md) alone does not establish it for arbitrary nonlinear problems.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

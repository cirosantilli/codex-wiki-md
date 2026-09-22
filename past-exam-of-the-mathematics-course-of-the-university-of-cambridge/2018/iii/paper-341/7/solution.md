<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

An $s$-stage [Runge-Kutta method](../../../../../runge-kutta-method.md) for $y'=f(t,y)$ is defined by

$$
Y_i=y_n+h\sum_{j=1}^sa_{ij}f(t_n+c_jh,Y_j),\qquad
y_{n+1}=y_n+h\sum_{i=1}^sb_if(t_n+c_ih,Y_i).
$$

The [Butcher tableau](../../../../../butcher-tableau.md) records $A=(a_{ij})$, $b$ and $c$; internal consistency usually sets $c=Ae$, and first-order consistency requires $b^Te=1$. A strictly lower triangular $A$ gives an explicit method, while other stage dependencies generally require an [implicit Runge-Kutta method](../../../../../implicit-runge-kutta-method.md). The [stage solvability of an implicit Runge-Kutta method](../../../../../stage-solvability-of-an-implicit-runge-kutta-method.md) must be checked separately: if $f$ is globally [Lipschitz continuous](../../../../../lipschitz-continuity.md) in $y$ with constant $L$, the stage fixed-point map is a contraction in the maximum stage norm whenever $hL\max_i\sum_j|a_{ij}|<1$. This is a sufficient small-step condition, not a restriction intrinsic to the definitions of [A-stability](../../../../../a-stability.md) or [B-stability](../../../../../b-stability.md).

Linear stability begins with the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$. Solving the stages gives

$$
\boxed{y_{n+1}=R(z)y_n,\qquad
R(z)=1+zb^T(I-zA)^{-1}e,\qquad z=h\lambda.}
$$

The [linear stability domain](../../../../../linear-stability-domain.md) consists of test values for which the stage system is well defined and $|R(z)|\leq1$. [A-stability](../../../../../a-stability.md) means this includes the closed left half-plane. For $\operatorname{Re}\lambda<0$, this gives stability with no scalar decay-mode step restriction. For a [normal matrix](../../../../../normal-matrix.md) $L$ in $y'=Ly$, [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md) reduces the [norm](../../../../../norm.md) estimate to these scalar factors. For a [non-normal matrix](../../../../../non-normal-matrix.md), eigenvalues alone do not establish a uniform [norm](../../../../../norm.md) bound: eigenvector conditioning and transient amplification matter. Mesh-uniform estimates for discretized PDEs must control operator powers, not only their spectra.

Every consistent explicit [Runge-Kutta method](../../../../../runge-kutta-method.md) has a nonconstant polynomial [stability function](../../../../../stability-function.md) and therefore cannot be [A-stable](../../../../../a-stability.md), since that polynomial is unbounded on the negative real axis. For example, [Forward Euler method](../../../../../euler-method.md) has $R(z)=1+z$, stability disk $|1+z|\leq1$, and restriction $0\leq hq\leq2$ for $\lambda=-q<0$. For a pure imaginary mode $\lambda=i\omega\neq0$, $|1+ih\omega|>1$, so it is unstable for every positive step. The [classical fourth-order Runge-Kutta method](../../../../../classical-fourth-order-runge-kutta-method.md) instead has

$$
R(z)=1+z+\tfrac12z^2+\tfrac16z^3+\tfrac1{24}z^4,
\qquad |R(iq)|^2=1-\frac{q^6}{72}+\frac{q^8}{576}.
$$

It is stable on the imaginary axis exactly for $|q|\leq2\sqrt2$, an illustrative conditional stability range for oscillatory evolution.

[Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=(1-z)^{-1}$ and is [A-stable](../../../../../a-stability.md). [L-stability](../../../../../l-stability.md) adds $R(z)\to0$ as $|z|\to\infty$ in the left half-plane; backward Euler satisfies this and strongly damps unresolved rapidly decaying modes in a [stiff differential equation](../../../../../stiff-equation.md). The [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) and the [trapezoidal rule](../../../../../trapezoidal-rule.md) both have $R(z)=(1+z/2)/(1-z/2)$, so they are [A-stable](../../../../../a-stability.md) but not [L-stable](../../../../../l-stability.md). They preserve the modulus of a pure imaginary test mode, but their stiff-decay limit is $-1$, leaving oscillatory numerical remnants. The three-stage [Lobatto IIIA method](../../../../../lobatto-iiia-method.md) has the fourth-order rational function found in Question 2 and likewise lacks [L-stability](../../../../../l-stability.md). Thus high order and [A-stability](../../../../../a-stability.md) do not themselves imply efficient stiff damping.

Nonlinear stability measures differences between solutions of the same equation. A [one-sided Lipschitz condition](../../../../../one-sided-lipschitz-condition.md) is

$$
\operatorname{Re}\langle f(t,y)-f(t,\widetilde y),y-\widetilde y\rangle
\leq\nu\|y-\widetilde y\|^2.
$$

Differentiating the squared difference and applying the [Gronwall inequality](../../../../../gronwall-inequality.md) gives $\|y(t)-\widetilde y(t)\|\leq e^{\nu(t-t_0)}\|y(t_0)-\widetilde y(t_0)\|$. A [dissipative vector field](../../../../../dissipative-vector-field.md) has $\nu\leq0$ and is contractive. A [B-stable](../../../../../b-stability.md) method preserves this property for every positive step size for which the stages are well defined:

$$
\boxed{\|y_{n+1}-\widetilde y_{n+1}\|\leq\|y_n-\widetilde y_n\|.}
$$

This includes time-dependent vector fields when dissipativity holds at each common time argument. Applying it to scalar linear dissipative fields shows that [B-stability](../../../../../b-stability.md) implies [A-stability](../../../../../a-stability.md) when the linear stages are well defined; the converse fails.

The standard sufficient theorem is **[algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) implies [B-stability](../../../../../b-stability.md)**, subject to stage solvability. Define $B=\operatorname{diag}(b)$ and $M=BA+A^TB-bb^T$. [Algebraic stability of a Runge-Kutta method](../../../../../algebraic-stability-of-a-runge-kutta-method.md) means $b_i\geq0$ and $M$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md). To prove the theorem, set $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$ and $F_i=f(t_n+c_ih,Y_i)-f(t_n+c_ih,\widetilde Y_i)$. Expanding the output difference and using $D_i=d+h\sum_ja_{ij}F_j$ yields the [Runge-Kutta contractivity identity](../../../../../runge-kutta-contractivity-identity.md)

$$
\|d_{n+1}\|^2=\|d\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

Dissipativity makes the first sum nonpositive, while positive semidefiniteness makes the last [quadratic form](../../../../../quadratic-form.md) nonnegative. The latter follows by factoring $M=Q^TQ$ and writing it as a sum of squared [norms](../../../../../norm.md) of linear combinations of the $F_i$. This proves the claimed contraction. It is a sufficient theorem; absence of [algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) is not, by itself, a proof of failure of [B-stability](../../../../../b-stability.md) for every representation.

Several examples make the distinctions concrete. For backward Euler, $b=1$, $A=(1)$, so $M=(1)$: it is both [L-stable](../../../../../l-stability.md) and [B-stable](../../../../../b-stability.md). For implicit midpoint, $b=1$, $A=(1/2)$, so $M=(0)$: it is [B-stable](../../../../../b-stability.md) and preserves squared [norms](../../../../../norm.md) for a skew-Hermitian linear equation, but lacks stiff damping. For the two-stage [Gauss--Legendre Runge-Kutta method](../../../../../gauss-legendre-method.md),

$$
A=\begin{pmatrix}1/4&1/4-\sqrt3/6\\1/4+\sqrt3/6&1/4\end{pmatrix},
\qquad b=(1/2,1/2)^T,
$$

the matrix $M$ vanishes as well. The collocation theorem gives order four, and its [stability function](../../../../../stability-function.md) is exactly the same as the three-stage Lobatto IIIA function. Yet the Gauss method is [algebraically stable](../../../../../algebraic-stability-of-a-runge-kutta-method.md), whereas that Lobatto method is not. Identical scalar linear stability functions need not imply identical nonlinear stability properties.

An example combining stiff damping and nonlinear contraction is the two-stage [Radau IIA method](../../../../../radau-iia-method.md), with

$$
A=\begin{pmatrix}5/12&-1/12\\3/4&1/4\end{pmatrix},\quad
b=(3/4,1/4)^T,\quad
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\quad
R(z)=\frac{1+z/3}{1-2z/3+z^2/6}.
$$

Its positive weights and positive semidefinite $M$ prove [B-stability](../../../../../b-stability.md); its rational function has denominator roots $2\pm i\sqrt2$ and, for $z=x+iy$, satisfies

$$
|1-2z/3+z^2/6|^2-|1+z/3|^2
=\frac{|z|^4-8x|z|^2+24x^2-72x}{36}\geq0\quad(x\leq0).
$$

Thus it is [A-stable](../../../../../a-stability.md); the limit $R(z)\to0$ then proves [L-stability](../../../../../l-stability.md). The standard Radau IIA collocation theorem gives order $2s-1$, here three. These properties explain its usefulness for stiff nonlinear equations.

Finally, **[A-stability](../../../../../a-stability.md) alone does not imply [B-stability](../../../../../b-stability.md)**. The [trapezoidal rule fails B-stability](../../../../../trapezoidal-rule-fails-b-stability.md) even for the scalar dissipative equation $y'=-y^3$. With $h=1$, its step map $T$ is uniquely defined by

$$
T(y)+\tfrac12T(y)^3=y-\tfrac12y^3.
$$

At $y=\sqrt2$, $T(y)=0$. Implicit differentiation gives

$$
T'(y)=\frac{1-\tfrac32y^2}{1+\tfrac32T(y)^2},\qquad T'(\sqrt2)=-2.
$$

Thus nearby starting values are separated by approximately twice their original distance after one step, although the exact flow is contractive. This example and the contractivity theorem show why scalar linear analysis, stiff damping and genuinely nonlinear [norm](../../../../../norm.md) estimates answer different stability questions.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

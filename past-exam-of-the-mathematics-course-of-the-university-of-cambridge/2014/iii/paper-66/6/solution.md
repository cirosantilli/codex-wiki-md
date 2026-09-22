<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [stiff differential equation](../../../../../stiff-equation.md) can contain rapidly decaying modes as well as a slowly changing solution of interest. An explicit scheme may need a very small step solely to keep those already small fast modes from numerical growth. [A-stability](../../../../../a-stability.md) addresses this restriction through the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$, whose exact solution decays when $\operatorname{Re}\lambda<0$.

For a one-step method, write $y_{n+1}=R(z)y_n$, $z=h\lambda$. Its [linear stability domain](../../../../../linear-stability-domain.md) consists of the points where the update is defined and $|R(z)|\leq1$. **[A-stability](../../../../../a-stability.md) means that this domain contains the closed left half-plane.** This is a scalar linear stability property, not an order condition, an existence theorem for an implicit solve, or a general nonlinear contractivity assertion.

For a rational approximation to the exponential, consistency requires $R(z)=1+z+O(z^2)$, and order $p$ requires $R(z)-e^z=O(z^{p+1})$. Poles must be absent from the relevant half-plane. The [Forward Euler method](../../../../../euler-method.md) has $R=1+z$ and the disk $|1+z|\leq1$, so negative real modes require $h|\lambda|\leq2$; it is not [A-stable](../../../../../a-stability.md). The [Backward Euler method](../../../../../backward-euler-method.md) has $R=(1-z)^{-1}$, and $|1-z|\geq1$ on the left half-plane, so it is [A-stable](../../../../../a-stability.md). The [trapezoidal rule](../../../../../trapezoidal-rule.md) and the [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) both have, on the scalar linear problem,

$$
R(z)=\frac{1+z/2}{1-z/2},\qquad
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z.
$$

They are second-order and [A-stable](../../../../../a-stability.md) despite being different nonlinear methods. No nonconstant polynomial approximation is [A-stable](../../../../../a-stability.md), because its modulus grows without bound on the negative real axis. In particular every nontrivial explicit [Runge-Kutta method](../../../../../runge-kutta-method.md) has a bounded-step stability restriction.

[A-stability](../../../../../a-stability.md) prevents growth but need not eliminate extremely stiff modes: the trapezoidal factor tends to minus one as $z\to-\infty$. [L-stability](../../../../../l-stability.md) additionally requires $R(z)\to0$ within the left half-plane. Backward Euler is [L-stable](../../../../../l-stability.md); trapezoidal and implicit midpoint are not. The distinction explains persistent alternating transients in otherwise stable Crank-Nicolson calculations. Accuracy still constrains useful step sizes even for an [A-stable](../../../../../a-stability.md) method.

A [linear multistep method](../../../../../linear-multistep-method.md) is characterized by polynomials $\rho,\sigma$, and its scalar modes satisfy $\rho(\zeta)-z\sigma(\zeta)=0$. There is generally no single scalar amplification factor: every root must lie in the closed unit disk and unit roots must be simple. At $z=0$, this is the [zero-stability](../../../../../zero-stability.md) root condition. Consistency plus [zero-stability](../../../../../zero-stability.md) gives convergence by the [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md), with suitable starting values. [A-stability](../../../../../a-stability.md) demands the amplification root condition throughout the left half-plane, including the zero-step condition. The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) says that an irreducible [A-stable](../../../../../a-stability.md) [linear multistep method](../../../../../linear-multistep-method.md) has order at most two, and an explicit [linear multistep method](../../../../../linear-multistep-method.md) cannot be [A-stable](../../../../../a-stability.md).

Examples include backward Euler, trapezoidal, and the second-order [backward differentiation formula](../../../../../backward-differentiation-formula.md)

$$
3y_{n+2}-4y_{n+1}+y_n=2hf(y_{n+2}).
$$

Its zero-step roots are $1,1/3$. Its unit-circle boundary quotient has real part $(1-\cos\theta)^2\geq0$, and the leading coefficient is nonzero on the left half-plane, giving [A-stability](../../../../../a-stability.md) by the same continuation argument as in Question 2. Conversely the third-order member of that question fails [A-stability](../../../../../a-stability.md). A formal high order without [zero-stability](../../../../../zero-stability.md), or after silently cancelling a problematic unit factor, does not evade the barrier.

For an [implicit Runge-Kutta method](../../../../../implicit-runge-kutta-method.md), the stages on the test equation satisfy $Y=e\,y_n+zAY$. Whenever these stages are solvable, its [stability function](../../../../../stability-function.md) is

$$
\boxed{R(z)=1+z\,b^T(I-zA)^{-1}e.}
$$

This rational function is used to test scalar [A-stability](../../../../../a-stability.md); the [Butcher order conditions](../../../../../butcher-order-condition.md) separately establish nonlinear order. The [Lobatto IIIA method](../../../../../lobatto-iiia-method.md) in Question 3 is an [A-stable](../../../../../a-stability.md) fourth-order example with $R$ the diagonal degree-two Padé approximant. More generally the $s$-stage [Gauss--Legendre Runge-Kutta method](../../../../../gauss-legendre-method.md) has order $2s$ and is [A-stable](../../../../../a-stability.md), with the diagonal Padé approximation to $e^z$; its stiff-limit factor is nonzero. The $s$-stage [Radau IIA method](../../../../../radau-iia-method.md) has order $2s-1$ and is [L-stable](../../../../../l-stability.md). Thus Runge-Kutta stages permit arbitrarily high [A-stable](../../../../../a-stability.md) order, unlike irreducible linear multistep formulas.

For a [normal matrix](../../../../../normal-matrix.md), scalar amplification bounds transfer through unitary diagonalization. For a [non-normal matrix](../../../../../non-normal-matrix.md), [eigenvalue](../../../../../eigenvalue.md) information alone does not assert Euclidean contraction: transient growth and eigenvector conditioning can matter. Direct [energy method](../../../../../energy-method.md) arguments, such as the dissipative Cayley-transform proof in Question 1, use the symmetric part and are more informative in that setting.

For nonlinear dissipative vector fields, the stronger [B-stability](../../../../../b-stability.md) property asks that distances between two numerical solutions not increase. A standard sufficient condition for [Runge-Kutta methods](../../../../../runge-kutta-method.md) is [algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md): $b_i\geq0$ and

$$
(b_i a_{ij}+b_j a_{ji}-b_i b_j)_{ij}
$$

is positive semidefinite. It follows from the [Runge-Kutta contractivity identity](../../../../../runge-kutta-contractivity-identity.md) when the implicit stages exist. The three-stage Lobatto IIIA method is [A-stable](../../../../../a-stability.md) but has the first diagonal entry of that [matrix](../../../../../matrix.md) equal to $-1/36$, so scalar [A-stability](../../../../../a-stability.md) should not be confused with that sufficient nonlinear condition. [Stage solvability of an implicit Runge-Kutta method](../../../../../stage-solvability-of-an-implicit-runge-kutta-method.md) remains a separate issue and computational cost of the implicit equations must be considered. **[A-stability](../../../../../a-stability.md) removes a scalar decay-mode stability restriction; order, stiff damping, nonlinear stability and solvability remain distinct properties.**

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

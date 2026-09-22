<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Runge-Kutta method](../../../../../runge-kutta-method.md) advances $y'=f(t,y)$ through stages

$$
Y_i=y_n+h\sum_j a_{ij}F_j,\qquad
F_j=f(t_n+c_jh,Y_j),\qquad
y_{n+1}=y_n+h\sum_i b_iF_i.
$$

The [Butcher tableau](../../../../../butcher-tableau.md) records $A,b,c$, normally with $c=Ae$. Linear [absolute stability](../../../../../linear-stability-domain.md) tests the amplification of a linear decay mode; nonlinear [B-stability](../../../../../b-stability.md) compares distances between two solutions of a [dissipative vector field](../../../../../dissipative-vector-field.md). Both describe propagation of perturbations, but they impose different conditions.

For the [Dahlquist test equation](../../../../../dahlquist-test-equation.md), elimination of stages gives

$$
R(z)=1+zb^T(I-zA)^{-1}e,\qquad z=h\lambda.
$$

The [linear stability domain](../../../../../linear-stability-domain.md) consists of $z$ for which the step is defined and $|R(z)|\leq1$. Poles or singular stage systems must be excluded, even if an output formula has a formal cancellation. For a scalar test equation, the proof is $y_n=R(z)^ny_0$: the powers are bounded exactly when $|R(z)|\leq1$. For $y'=Ly$, the update is $R(hL)$. If $L$ is a [normal matrix](../../../../../normal-matrix.md), [unitary diagonalization of a normal matrix](../../../../../unitary-diagonalization-of-a-normal-matrix.md) makes the [operator norm](../../../../../operator-norm.md) equal to the largest scalar amplification [modulus](../../../../../modulus.md). For a diagonalizable [matrix](../../../../../matrix.md), powers are bounded by the [condition number](../../../../../condition-number.md) of the [eigenvector](../../../../../eigenvector.md) matrix times the maximal scalar power. These constants must remain uniform for mesh-dependent systems. A defective unit-modulus [eigenvalue](../../../../../eigenvalue.md) can instead produce a growing [Jordan block](../../../../../jordan-block.md); the scalar spectral test alone does not control a general [matrix](../../../../../matrix.md).

An [A-stable](../../../../../a-stability.md) method accepts the entire closed left half-plane. The [Explicit Euler method](../../../../../euler-method.md) has $R(z)=1+z$ and a disk of stability $|1+z|\leq1$, so it is not [A-stable](../../../../../a-stability.md). No nonconstant [polynomial](../../../../../polynomial-split.md) [stability function](../../../../../stability-function.md) can be [A-stable](../../../../../a-stability.md), since it is unbounded on the negative real axis; this excludes all consistent explicit [Runge-Kutta methods](../../../../../runge-kutta-method.md). The [Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=1/(1-z)$, and $|1-z|\geq1$ when $\operatorname{Re}z\leq0$, proving [A-stability](../../../../../a-stability.md). It is also [L-stable](../../../../../l-stability.md), because $R(z)\to0$ for large left-half-plane $z$.

The [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) and the [trapezoidal rule](../../../../../trapezoidal-rule.md) have the same scalar [stability function](../../../../../stability-function.md),

$$
R(z)=\frac{1+z/2}{1-z/2}.
$$

The identity $|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z$ proves [A-stability](../../../../../a-stability.md). On the imaginary axis their amplification has unit [modulus](../../../../../modulus.md), and along the negative real axis it tends to $-1$. Thus neither is [L-stable](../../../../../l-stability.md); very stiff decay can persist as alternating numerical values. In contrast, the two-stage [Radau IIA method](../../../../../radau-iia-method.md) has $R(z)=(1+z/3)/(1-2z/3+z^2/6)$, with the explicit nonnegative modulus-gap proof in question 1, and is [L-stable](../../../../../l-stability.md). This illustrates why [L-stability](../../../../../l-stability.md) matters beyond [A-stability](../../../../../a-stability.md) for a [stiff differential equation](../../../../../stiff-equation.md).

For nonlinear problems, assume a real or complex Euclidean [inner product](../../../../../inner-product.md) and the dissipativity hypothesis

$$
\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0
$$

for all relevant states at each common time. Exact solutions satisfy

$$
\frac{d}{dt}\|u-v\|^2
=2\operatorname{Re}\langle f(t,u)-f(t,v),u-v\rangle\leq0.
$$

A [B-stable](../../../../../b-stability.md) [Runge-Kutta method](../../../../../runge-kutta-method.md) reproduces this nonexpansion of distances whenever its stages exist. Put $d=y_n-\widetilde y_n$, $D_i=Y_i-\widetilde Y_i$, and $G_i=f(t_n+c_ih,Y_i)-f(t_n+c_ih,\widetilde Y_i)$. Then $D_i=d+h\sum_j a_{ij}G_j$. Expansion of the output squared [norm](../../../../../norm.md), followed by substituting $d=D_i-h\sum_j a_{ij}G_j$ in its linear terms, proves the [Runge-Kutta contractivity identity](../../../../../runge-kutta-contractivity-identity.md)

$$
\|d_{\mathrm{new}}\|^2-\|d\|^2
=2h\sum_i b_i\operatorname{Re}\langle D_i,G_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle G_i,G_j\rangle,
\quad
m_{ij}=b_i a_{ij}+b_j a_{ji}-b_i b_j.
$$

If $b_i\geq0$ and $M=(m_{ij})$ is a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), the first sum is nonpositive by dissipativity, and the second is nonnegative: expand each coordinate of the stage [vectors](../../../../../vector.md) to express it as a sum of nonnegative [quadratic forms](../../../../../quadratic-form.md). These are exactly the conditions for [algebraic stability of a Runge-Kutta method](../../../../../algebraic-stability-of-a-runge-kutta-method.md). Hence **[algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) implies [B-stability](../../../../../b-stability.md)**. Applying [B-stability](../../../../../b-stability.md) to the linear dissipative problem $y'=\lambda y$, or its two-dimensional real form, also proves [A-stability](../../../../../a-stability.md) whenever stages are well defined.

The [Backward Euler method](../../../../../backward-euler-method.md) has $b=A=1$, hence $M=1$; the [implicit midpoint rule](../../../../../implicit-midpoint-rule.md) has $b=1$, $A=1/2$, hence $M=0$. Both are [algebraically stable](../../../../../algebraic-stability-of-a-runge-kutta-method.md) and [B-stable](../../../../../b-stability.md). For the two-stage [Radau IIA method](../../../../../radau-iia-method.md),

$$
M=\frac1{16}\begin{pmatrix}1&-1\\-1&1\end{pmatrix},
$$

a [positive semidefinite matrix](../../../../../positive-semidefinite-matrix.md), while both weights are positive. It therefore combines third-order accuracy, [B-stability](../../../../../b-stability.md), and [L-stability](../../../../../l-stability.md). The distinction between stability and solvability is essential: for [Lipschitz continuous](../../../../../lipschitz-continuity.md) $f$, the stage map is a contraction when $hL\max_i\sum_j|a_{ij}|<1$, so the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) proves small-step unique solvability. The preceding [algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) proof is an estimate for existing stages; it is not a theorem asserting stage existence for arbitrary step sizes and domains.

Linear [A-stability](../../../../../a-stability.md) is insufficient for nonlinear [B-stability](../../../../../b-stability.md). The [trapezoidal rule fails B-stability](../../../../../trapezoidal-rule-fails-b-stability.md), even though its scalar [stability function](../../../../../stability-function.md) is identical to that of the [B-stable](../../../../../b-stability.md) [implicit midpoint rule](../../../../../implicit-midpoint-rule.md). Its [Runge-Kutta method](../../../../../runge-kutta-method.md) coefficients are

$$
A=\begin{pmatrix}0&0\\1/2&1/2\end{pmatrix},\qquad
b=(1/2,1/2)^T,\qquad
M=\begin{pmatrix}-1/4&0\\0&1/4\end{pmatrix}.
$$

Failure of this sufficient [algebraic stability](../../../../../algebraic-stability-of-a-runge-kutta-method.md) test alone would not prove failure of [B-stability](../../../../../b-stability.md). An actual counterexample does: take $f(y)=-y^3$ and $h=2$. Dissipativity follows from

$$
(f(u)-f(v))(u-v)=-(u-v)^2(u^2+uv+v^2)\leq0.
$$

The unique step map $T$ obeys $T+T^3=y-y^3$, because the left-hand side is strictly increasing and onto. At $y=1$, $T=0$, and implicit [differentiation](../../../../../differentiation.md) gives

$$
T'(1)=\frac{1-3(1)^2}{1+3T(1)^2}=-2.
$$

Nearby initial states expand in distance. This proves a true nonlinear failure rather than merely failure of a coefficient criterion.

Finally, [stability of a numerical method](../../../../../stability-of-a-numerical-method.md) on finite intervals connects these contractivity properties to accuracy. If a one-step map is nonexpansive and its exact one-step defect has [norm](../../../../../norm.md) at most $Ch^{p+1}$, then the error satisfies $\|e_{n+1}\|\leq\|e_n\|+Ch^{p+1}$, hence $\|e_n\|\leq\|e_0\|+CT h^p$ for $nh\leq T$. A Lipschitz step bound $1+Kh$ gives the same order using the [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md). For a [stiff differential equation](../../../../../stiff-equation.md), the value of [B-stability](../../../../../b-stability.md) is that the propagation estimate need not grow with a large negative dissipative rate. The accuracy constant still needs appropriate smoothness and uniform [derivative](../../../../../derivative.md) bounds; stability alone does not establish a mesh-uniform error order.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 341](../../paper-341-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

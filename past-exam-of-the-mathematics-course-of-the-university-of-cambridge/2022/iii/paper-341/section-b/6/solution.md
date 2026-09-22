<h1 id="section-b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

An $s$-stage [Runge-Kutta method](../../../../../../runge-kutta-method.md) has stages and update

$$
Y_i=y_n+h\sum_{j=1}^sa_{ij}f(Y_j),
\qquad
y_{n+1}=y_n+h\sum_{i=1}^sb_if(Y_i).
$$

On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md) $y'=\lambda y$, elimination of the stages gives the [stability function](../../../../../../stability-function.md)

$$
R(z)=1+z b^T(I-zA)^{-1}\mathbf1,
\qquad z=h\lambda.
$$

The [linear stability domain](../../../../../../linear-stability-domain.md) is the set where $|R(z)|\leq1$. A method is [A-stable](../../../../../../a-stability.md) when this domain contains $\operatorname{Re}z\leq0$, so every exactly decaying scalar linear mode remains bounded for every step size. It is [L-stable](../../../../../../l-stability.md) when it is A-stable and $R(z)\to0$ as $|z|\to\infty$ in the left half-plane; this extra limit strongly damps unresolved stiff modes.

The rational function $R$ makes several useful conclusions immediate. No explicit Runge--Kutta method is A-stable because its stability function is a nonconstant [polynomial](../../../../../../polynomial-split.md) and is therefore unbounded on the negative real axis. The [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md) has $R(z)=(1+z/2)/(1-z/2)$ and is A-stable, but $R(z)\to-1$, so it is not L-stable. The [Backward Euler method](../../../../../../backward-euler-method.md) has $R(z)=(1-z)^{-1}$ and is L-stable. More generally, a rational $R$ with no pole in the closed left half-plane is A-stable if and only if $|R(iy)|\leq1$ for every real $y$; this follows by applying the [maximum modulus principle](../../../../../../maximum-modulus-principle.md) on expanding left half-disks.

Scalar linear stability does not by itself control nonlinear perturbations. Suppose the vector field is dissipative in the sense that

$$
\operatorname{Re}\langle f(u)-f(v),u-v\rangle\leq0.
$$

A method is [B-stable](../../../../../../b-stability.md) if it preserves the resulting contractivity: two numerical solutions satisfy $\|y_{n+1}-\widetilde y_{n+1}\|\leq\|y_n-\widetilde y_n\|$. A practical sufficient condition is [algebraic stability of a Runge-Kutta method](../../../../../../algebraic-stability-of-a-runge-kutta-method.md): $b_i\geq0$ and

$$
M=BA+A^TB-bb^T\succeq0,
\qquad B=\operatorname{diag}(b_i).
$$

To prove the implication, let $D_i=Y_i-\widetilde Y_i$ and $F_i=f(Y_i)-f(\widetilde Y_i)$. Expanding the squared distance and substituting the stage equations gives the [Runge-Kutta contractivity identity](../../../../../../runge-kutta-contractivity-identity.md)

$$
\|y_{n+1}-\widetilde y_{n+1}\|^2
=\|y_n-\widetilde y_n\|^2
+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle
-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

The dissipativity inequalities make the middle sum nonpositive, and positive semidefiniteness of $M$ makes the final quadratic form nonnegative before its minus sign. The distance therefore cannot increase. In particular, algebraic stability implies B-stability and, by applying contractivity to the real two-dimensional form of $y'=\lambda y$, implies A-stability.

Important collocation families illustrate these notions. [Gauss methods](../../../../../../gauss-legendre-method.md) are A-stable, symmetric, and have order $2s$, but they do not damp infinitely stiff modes. [Radau IIA methods](../../../../../../radau-iia-method.md) have order $2s-1$, are algebraically stable, and are L-stable. These properties explain why A-stability controls unrestricted linear decay, L-stability is useful for stiff transients, and algebraic or B-stability is the stronger tool for nonlinear dissipative equations.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [Section B](../../section-b.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**A-stability removes the scalar linear decay restriction on the step size; it does not replace accuracy, nonlinear solvability or a suitable system norm.** Its importance is clearest for a [stiff differential equation](../../../../../stiff-equation.md), where rapidly decaying modes coexist with slowly varying quantities of interest. On the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$, the exact solution decays for $\operatorname{Re}\lambda<0$. A stable time integrator should not turn that decay into numerical growth.

For a one-step method write $y_{n+1}=R(z)y_n$, where $z=h\lambda$ and $R$ is its [stability function](../../../../../stability-function.md). Its [linear stability domain](../../../../../linear-stability-domain.md) consists of parameters with $|R(z)|\le1$ and a well-defined update. The method is [A-stable](../../../../../a-stability.md) when this domain contains the closed left half-plane. A consistent order-$p$ one-step method has $R(z)=e^z+O(z^{p+1})$ near zero, but that local agreement alone says nothing about stability at large negative $z$.

For a [Runge-Kutta method](../../../../../runge-kutta-method.md) with stage [matrix](../../../../../matrix.md) $A$, weights $b$ and $\mathbf1=(1,\ldots,1)^T$, eliminating the stages on the test equation gives

$$
R(z)=1+zb^T(I-zA)^{-1}\mathbf1.
$$

An explicit finite-stage method has a [polynomial](../../../../../polynomial-split.md) $R$. A nonconstant [polynomial](../../../../../polynomial-split.md) is unbounded along the negative real axis, so **no consistent explicit [Runge-Kutta method](../../../../../runge-kutta-method.md) is A-stable**. The [explicit Euler method](../../../../../euler-method.md), with $R(z)=1+z$, is stable in the disk $|1+z|\le1$ and on the negative real axis only for $-2\le z\le0$. A stiff mode with a large negative [eigenvalue](../../../../../eigenvalue.md) therefore forces an unnecessarily small step even after its exact contribution has almost disappeared.

The [Backward Euler method](../../../../../backward-euler-method.md) has $R(z)=1/(1-z)$. For $\operatorname{Re}z\le0$, $|1-z|^2=1-2\operatorname{Re}z+|z|^2\ge1$, so it is [A-stable](../../../../../a-stability.md). The [trapezoidal rule](../../../../../trapezoidal-rule.md) has

$$
R(z)=\frac{1+z/2}{1-z/2},\qquad
|1-z/2|^2-|1+z/2|^2=-2\operatorname{Re}z\ge0,
$$

and is also [A-stable](../../../../../a-stability.md). The [implicit midpoint method](../../../../../implicit-midpoint-rule.md) has the same scalar [stability function](../../../../../stability-function.md), although its nonlinear update differs from the trapezoidal rule. The first method has order one and the latter two order two. Their implicit solves trade greater work per step for freedom from the scalar stiff stability restriction.

<a id="6/image-absolute-stability-domains-of-explicit-euler-backward-euler-and-the-trapezoidal-rule-shaded-regions-satisfy-modulus-of-the-amplification-factor-at-most-one"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63-stability-domains.png)

**[Figure 1](#6/image-absolute-stability-domains-of-explicit-euler-backward-euler-and-the-trapezoidal-rule-shaded-regions-satisfy-modulus-of-the-amplification-factor-at-most-one). Absolute stability domains of explicit Euler, backward Euler and the trapezoidal rule; shaded regions satisfy modulus of the amplification factor at most one**.

Damping of very stiff modes separates [A-stability](../../../../../a-stability.md) from [L-stability](../../../../../l-stability.md). For a one-step method, the latter additionally requires $R(z)\to0$ as $z$ tends to infinity in the left half-plane. [Backward Euler method](../../../../../backward-euler-method.md) satisfies this. The trapezoidal and midpoint rules instead have $R(z)\to-1$ along the negative real axis: a very stiff mode can alternate in sign with little damping even though its amplitude remains bounded. [L-stability](../../../../../l-stability.md) is often preferable for diffusion and rapid relaxation, while retaining oscillatory modes can be desirable in conservative dynamics.

For a [linear multistep method](../../../../../linear-multistep-method.md), write

$$
\sum_{j=0}^k\alpha_jy_{n+j}=h\sum_{j=0}^k\beta_jf_{n+j},\qquad
\rho(\zeta)=\sum_j\alpha_j\zeta^j,\quad \sigma(\zeta)=\sum_j\beta_j\zeta^j.
$$

Its test-equation amplification roots satisfy $\rho(\zeta)-z\sigma(\zeta)=0$. [Absolute stability](../../../../../linear-stability-domain.md) requires every root to lie in the [unit disk](../../../../../unit-disk.md) or on its boundary with all unit-modulus roots simple; all parasitic modes matter. At $z=0$ this is the [zero-stability](../../../../../zero-stability.md) root condition. Consistency requires $\rho(1)=0$ and $\rho'(1)=\sigma(1)$, and the [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) combines consistency and [zero-stability](../../../../../zero-stability.md) to characterize convergence. Thus a claim of stability obtained by canceling a common factor is not a proof about the original recurrence and its arbitrary consistent starting data.

Explicit [linear multistep methods](../../../../../linear-multistep-method.md) cannot be [A-stable](../../../../../a-stability.md) either. If $\beta_k=0$ and $\alpha_k\ne0$, some lower coefficient of $\rho-z\sigma$ becomes unbounded as $z\to-\infty$, while the leading coefficient stays fixed. If all roots remained in the [unit disk](../../../../../unit-disk.md), every coefficient-to-leading-coefficient ratio, an elementary symmetric function of those roots, would remain bounded. This contradiction forces an unstable root.

An important implicit example is [BDF2 method](../../../../../second-order-backward-differentiation-formula.md), whose characteristic equation is $(3-2z)\zeta^2-4\zeta+1=0$. A unit root $\zeta=e^{i\theta}$ gives

$$
z(\theta)=\tfrac12(3-4e^{-i\theta}+e^{-2i\theta}),\qquad
\operatorname{Re}z(\theta)=(1-\cos\theta)^2\ge0.
$$

The leading coefficient vanishes only at $z=3/2$, outside the left half-plane. Near a small negative $z$, both roots are inside the disk; no unit-circle crossing can occur in the connected open left half-plane. On the imaginary axis the boundary equality can occur only at $z=0$, where the roots are $1,1/3$. Hence BDF2 is [A-stable](../../../../../a-stability.md) and its two roots tend to zero for very large negative $z$, giving strong stiff-mode damping. This is a complete boundary-locus argument, not just a boundary plot.

The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) says that a convergent [A-stable](../../../../../a-stability.md) ordinary [linear multistep method](../../../../../linear-multistep-method.md) has order at most two. This theorem does not limit [implicit Runge-Kutta methods](../../../../../implicit-runge-kutta-method.md) or [multiderivative multistep methods](../../../../../multiderivative-multistep-method.md). In particular the [A-stable third-order two-step multiderivative method](../../../../../a-stable-third-order-two-step-multiderivative-method.md) in question 1 uses $y''$ and satisfies different order conditions. Among [collocation Runge-Kutta methods](../../../../../collocation-runge-kutta-method.md), the standard family results give [Gauss collocation methods](../../../../../gauss-legendre-method.md) order $2s$ with diagonal $[s/s]$ [Padé approximants](../../../../../pade-approximant.md) to $e^z$ as [stability functions](../../../../../stability-function.md), and [Radau IIA methods](../../../../../radau-iia-method.md) order $2s-1$ with subdiagonal $[s-1/s]$ approximants. Both families are [A-stable](../../../../../a-stability.md); the Gauss functions have a nonzero limit at infinity, whereas Radau IIA is [L-stable](../../../../../l-stability.md). The corrected two-stage right-Radau method, for example, has

$$
R(z)=\frac{1+z/3}{1-2z/3+z^2/6},
$$

which matches the exponential through cubic order and tends to zero at infinity. Its poles $2\pm i\sqrt2$ lie in the right half-plane. For $z=-r+iy$, $r\ge0$, direct subtraction gives

$$
|1-2z/3+z^2/6|^2-|1+z/3|^2
=\frac{r(r+6)(r^2+2r+12)+2r(r+4)y^2+y^4}{36}\ge0,
$$

proving its [A-stability](../../../../../a-stability.md) directly.

Sectorial [A-alpha stability](../../../../../a-alpha-stability.md) relaxes the requirement to a sector around the negative real axis, useful when the spectrum of a stiff problem remains in that sector; higher-order backward differentiation formulas illustrate the usefulness of this weaker requirement. For a normal linear system $y'=Ly$, unitary diagonalization reduces the numerical update to its scalar factors $R(h\lambda_j)$. For a nonnormal system, a scalar [eigenvalue](../../../../../eigenvalue.md) test alone does not give a uniform bound in the chosen norm. Nonlinear stability is different again: [B-stability](../../../../../b-stability.md) asks for contractivity when $\operatorname{Re}\langle f(u)-f(v),u-v\rangle\le0$, and [algebraic stability of a Runge-Kutta method](../../../../../algebraic-stability-of-a-runge-kutta-method.md) is a standard sufficient criterion. Thus [A-stability](../../../../../a-stability.md) addresses a precise and valuable linear test, while step selection still has to meet accuracy requirements and the actual implicit equations must be solved on the relevant branch.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

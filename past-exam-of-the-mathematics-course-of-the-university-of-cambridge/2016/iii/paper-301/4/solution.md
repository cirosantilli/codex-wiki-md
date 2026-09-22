<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Return to the mostly-minus [Minkowski metric](../../../../../minkowski-metric.md) of Question 3, and write $f=\partial_aA^a$. The field $\xi(x)$ is assumed real and nonzero wherever its inverse occurs. Under the usual Abelian [gauge transformation](../../../../../gauge-transformation.md) $A_a\mapsto A_a+\partial_a\lambda$, with $\xi$ inert, the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) is invariant but $f\mapsto f+\Box\lambda$. The change in the added density is

$$
\Delta\mathcal L=\frac{f\Box\lambda}{\xi}+\frac{(\Box\lambda)^2}{2\xi}.
$$

This is not generally a total derivative. **The action is not invariant under arbitrary gauge transformations.** It retains [residual Lorenz gauge symmetry](../../../../../residual-lorenz-gauge-symmetry.md) for transformations satisfying $\Box\lambda=0$, with the same [boundary conditions](../../../../../boundary-condition.md) imposed before and after the transformation. The action itself is undefined at $\xi=0$; that value can only be considered as a limiting gauge.

To vary the [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md), use $\delta F_{ab}=\partial_a\delta A_b-\partial_b\delta A_a$ and $\delta f=\partial_a\delta A^a$. The [integration by parts](../../../../../integration-by-parts.md) of both terms gives

$$
\delta_A S=\int d^4x\left[\partial_aF^{ab}-\partial^b\left(\frac f\xi\right)\right]\delta A_b,
$$

with surface terms removed by the variational [boundary conditions](../../../../../boundary-condition.md). Hence

$$
\boxed{\partial_aF^{ab}-\partial^b\left(\frac{\partial_cA^c}{\xi}\right)=0}.
$$

For variable $\xi$, the derivative must act on $1/\xi$ as well as on $f$:

$$
\Box A^b-\left(1+\frac1\xi\right)\partial^bf+\frac f{\xi^2}\partial^b\xi=0.
$$

Since $\xi$ enters algebraically, its [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is

$$
\boxed{-\frac{f^2}{2\xi^2}=0}.
$$

For a real field this gives $f=0$. Thus a [dynamical gauge-fixing parameter](../../../../../dynamical-gauge-fixing-parameter.md) imposes a [constraint equation in field theory](../../../../../constraint-equation-in-field-theory.md); it is not an ordinary propagating scalar. On configurations satisfying both equations, $\partial_aF^{ab}=0$, $\partial_aA^a=0$, and therefore $\Box A^b=0$. There is no independent kinetic equation that determines $\xi$.

For the momentum-space equation at a prescribed constant $\xi\ne0$, use $A_a(x)=\int d^4p\,e^{-ip\cdot x}A_a(p)/(2\pi)^4$. Then $\partial_a\mapsto-ip_a$, and the linear $A$ equation is

$$
\boxed{K^{ab}(p)A_b(p)=0},\qquad
K^{ab}(p)=-p^2\eta^{ab}+\left(1+\frac1\xi\right)p^ap^b.
$$

Equivalently, $-p^2A^a+(1+1/\xi)p^a(p\cdot A)=0$. If the separately varied $\xi$ equation is also imposed on a real classical solution, then $p\cdot A=0$ and its nonzero modes lie on the massless [mass shell](../../../../../mass-shell.md). For constructing a full-field [Green function](../../../../../green-s-function.md), however, invert the fixed-background quadratic operator before imposing that on-shell constraint. Holding $\xi$ fixed and integrating over $A$ is a [Gaussian functional integral](../../../../../gaussian-functional-integral.md); integrating over the original variable $\xi$ as well is a different constrained problem.

For $p^2\ne0$, the Lorentzian versions of the [transverse projector of a vector field](../../../../../transverse-projector-of-a-vector-field.md) and [longitudinal projector of a vector field](../../../../../longitudinal-projector-of-a-vector-field.md) are

$$
(P_L)^a{}_b=\frac{p^ap_b}{p^2},\qquad
(P_T)^a{}_b=\delta^a_b-(P_L)^a{}_b.
$$

They satisfy $P_T^2=P_T$, $P_L^2=P_L$, $P_TP_L=0$ and $P_T+P_L=I$. The mixed-index operator is

$$
K^a{}_b=-p^2(P_T)^a{}_b+\frac{p^2}{\xi}(P_L)^a{}_b.
$$

Its inverse follows by inverting these two scalar eigenvalues. Define $G_{ab}$ by $K^{ac}G_{cb}=\delta^a_b$. The [positive-sign covariant gauge-fixing inverse](../../../../../positive-sign-covariant-gauge-fixing-inverse.md) is

$$
\boxed{G_{ab}(p)=-\frac{\eta_{ab}}{p^2}+\frac{1+\xi}{(p^2)^2}p_ap_b},\qquad
G^{ab}(p)=-\frac{\eta^{ab}}{p^2}+\frac{1+\xi}{(p^2)^2}p^ap^b.
$$

This is the algebraic inverse of the kinetic operator. A vacuum [photon propagator](../../../../../photon-propagator.md) instead has the factor $iG_{ab}$ and a [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) for its simple and double poles. If the name $G$ is used for the vacuum two-point function, include that factor $i$ consistently in its defining source equation. A [retarded Green function](../../../../../retarded-green-function.md) would use different boundary conditions at the same poles. The original plus sign corresponds to the usual [covariant gauge](../../../../../covariant-gauge.md) parameter $\alpha=-\xi$; in particular, $\xi=-1$ gives [Feynman gauge](../../../../../feynman-gauge.md) and $G_{ab}=-\eta_{ab}/p^2$.

Contracting gives the [longitudinal gauge propagator contraction](../../../../../longitudinal-gauge-propagator-contraction.md)

$$
\boxed{p^aG_{ab}(p)=\frac{\xi p_b}{p^2}}.
$$

Thus the contraction is not identically zero as a function of [four-momentum](../../../../../four-momentum.md) for any $\xi\ne0$, and it is a nonzero vector at every nonzero non-null [four-momentum](../../../../../four-momentum.md). A particular component may vanish when $p_b=0$. At $p^2=0$, the displayed inverse has poles and must be interpreted using the chosen [Green function](../../../../../green-s-function.md) prescription, rather than as a pointwise finite matrix. In the limiting [covariant Landau gauge](../../../../../landau-gauge-quantum-field-theory.md), $\xi\to0$, the longitudinal part vanishes. **A covariant photon Green function may have a longitudinal component even though physical photon polarizations are transverse.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

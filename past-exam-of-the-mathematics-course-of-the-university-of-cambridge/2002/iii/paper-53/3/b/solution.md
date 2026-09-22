<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At rest the tensor equation relaxes $A$ toward $I$ and the stretch equation relaxes $\lambda$ toward one. Thus

$$
\boxed{A_0=I,\qquad B_0=\frac I3,\qquad\lambda_0=1.}
$$

The equilibrium nonpressure [stress](../../../../../../stress.md) $GI/3$ is isotropic and can be absorbed into the arbitrary [pressure](../../../../../../pressure.md) in [incompressible flow](../../../../../../incompressible-flow.md).

For the linear response, put $A=I+a+O(\varepsilon^2)$, $\lambda=1+\ell+O(\varepsilon^2)$ and take the [velocity gradient](../../../../../../velocity-gradient.md) to be $O(\varepsilon)$. The first-order tensor equation is

$$
D_ta+\frac a{\tau_1}=K+K^T=A_1.
$$

Its [matrix trace](../../../../../../matrix-trace.md) has no forcing, because [incompressibility](../../../../../../incompressible-flow.md) gives $\operatorname{tr}K=0$. Starting relaxed, $\operatorname{tr}a=0$. The first-order stretch equation is $D_t\ell+\ell/\tau_2=(I/3):K=0$, hence $\ell=0$. Consequently $B=I/3+a/3+O(\varepsilon^2)$, and its anisotropic [stress](../../../../../../stress.md) is $Ga/3$. From the relaxed remote past,

$$
\sigma^{\rm lin}=-p_*I+\frac G3\int_{-\infty}^t e^{-(t-s)/\tau_1}A_1(s)ds
=-p_*I+2\int_{-\infty}^t\frac G3e^{-(t-s)/\tau_1}E(s)ds.
$$

The [linear and second-order response of the differential pom-pom model](../../../../../../linear-and-second-order-response-of-the-differential-pom-pom-model.md) therefore has

$$
\boxed{G_{\rm rel}(t)=\frac G3e^{-t/\tau_1}\quad(t\ge0),\qquad\mu_0=\int_0^\infty G_{\rm rel}(t)dt=\frac{G\tau_1}{3}.}
$$

The stretch time $\tau_2$ does not enter the linear shear [relaxation modulus](../../../../../../relaxation-modulus.md).

For the [second-order fluid](../../../../../../second-order-fluid.md) constants, additionally make the slow-flow expansion: count $K$ as first order and $D_t$ as raising the order by one. Iterating

$$
A-I=\tau_1(KA+AK^T-D_tA)
$$

gives

$$
A=I+\tau_1A_1+\tau_1^2(KA_1+A_1K^T-D_tA_1)+O(3).
$$

Using the [Rivlin-Ericksen tensor](../../../../../../rivlin-ericksen-tensor.md) convention $A_2=D_tA_1+A_1K+K^TA_1$, the identity

$$
KA_1+A_1K^T+A_1K+K^TA_1=2A_1^2
$$

reduces this to $A=I+\tau_1A_1+\tau_1^2(2A_1^2-A_2)+O(3)$. Since $\operatorname{tr}A_2=\operatorname{tr}A_1^2$, normalization gives

$$
B=\frac I3+\frac{\tau_1}{3}A_1+\frac{\tau_1^2}{3}(2A_1^2-A_2)
-\frac{\tau_1^2}{9}\operatorname{tr}(A_1^2)I+O(3).
$$

Stretch first changes at second order. Its equation gives $\lambda-1=\tau_1\tau_2\operatorname{tr}(A_1^2)/6+O(3)$. Multiplication by $\lambda^2$ therefore adds only an isotropic [stress](../../../../../../stress.md) at second order; multiplying its second-order increment by the anisotropic first-order term would be third order. Absorb these isotropic corrections into $p_*$ to obtain

$$
\sigma=-p_*I+\frac{G\tau_1}{3}A_1+\frac{G\tau_1^2}{3}(2A_1^2-A_2)+O(3).
$$

Comparison with the [viscometric functions](../../../../../../viscometric-functions.md) parametrization yields

$$
\boxed{\mu_0=\frac{G\tau_1}{3},\qquad\psi_1=\frac{2G\tau_1^2}{3},\qquad\psi_2=0.}
$$

Equivalently, in $\sigma=-pI+\mu_0A_1+\alpha_1A_2+\alpha_2A_1^2$, the constants are $\alpha_1=-G\tau_1^2/3$ and $\alpha_2=2G\tau_1^2/3$. The general small-amplitude linear response above permits fast oscillation; the local [second-order fluid](../../../../../../second-order-fluid.md) expansion also requires the slow-flow ordering just used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

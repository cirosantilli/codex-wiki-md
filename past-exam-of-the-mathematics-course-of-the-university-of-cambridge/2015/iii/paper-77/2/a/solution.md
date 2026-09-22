<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Fourier transform](../../../../../../fourier-transform.md) convention $\widehat p(k,y)=\int_{\mathbb R}e^{ikx}p(x,y)dx$. Let $\gamma(k)^2=k^2-k_0^2$, choosing $\operatorname{Re}\gamma>0$ on the real contour with $\operatorname{Im}\omega<0$. For time dependence $e^{i\omega t}$, this is the decaying continuation of the outgoing [Sommerfeld radiation condition](../../../../../../sommerfeld-radiation-condition.md).

The transformed [Helmholtz equation](../../../../../../helmholtz-equation.md) has upper and lower solutions $P(k)e^{-\gamma y}$ and $Q(k)e^{\gamma y}$. The two kinematic traces give $-\gamma P=\rho_0\omega^2\widehat\eta=\gamma Q$, hence

$$
Q=-P,\qquad P=-\frac{\rho_0\omega^2}{\gamma}\widehat\eta,\qquad[\widehat p]=-\frac{2\rho_0\omega^2}{\gamma}\widehat\eta.
$$

The [elastic membrane](../../../../../../elastic-membrane.md) equation gives $[\widehat p]=(m\omega^2-Tk^2)\widehat\eta$. Therefore the [acoustic wave on a tensioned massive membrane](../../../../../../acoustic-wave-on-a-tensioned-massive-membrane.md) has [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{D(\omega,k)=m\omega^2-Tk^2+\frac{2\rho_0\omega^2}{\gamma(k)}=0.}
$$

Equivalently, $Tk^2=\omega^2(m+2\rho_0/\gamma)$. The fluid on both sides supplies a positive [added mass of an evanescent fluid layer](../../../../../../added-mass-of-an-evanescent-fluid-layer.md), which is a useful independent check on the sign. In particular, the incident [pressure](../../../../../../pressure.md) is

$$
p_I(x,y)=-\operatorname{sgn}(y)\frac{\rho_0\omega^2}{\gamma_I}e^{-ik_Ix-\gamma_I|y|},\qquad\gamma_I=\gamma(k_I).
$$

The symbol $m$ here denotes [elastic membrane](../../../../../../elastic-membrane.md) mass per area, rather than the fluctuating [Mach number](../../../../../../mach-number.md) used in Question 1.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

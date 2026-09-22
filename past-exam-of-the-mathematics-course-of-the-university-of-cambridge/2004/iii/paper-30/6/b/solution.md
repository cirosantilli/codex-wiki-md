<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply Q5(b) in each independent coordinate, with $\mu=\lambda$, to change from the Ornstein-Uhlenbeck path law to d-dimensional [Wiener measure](../../../../../../wiener-measure.md) $\mathbb Q^x$. Its density is

$$
\exp\!\left(-\lambda\int_0^t\omega_s\cdot d\omega_s
-\frac{\lambda^2}{2}\int_0^t|\omega_s|^2ds\right).
$$

Multiplication by the positive potential factor cancels the second term exactly. Therefore

$$
\boxed{u(t,x)=\int\exp\!\left(-\lambda\int_0^t\omega_s\cdot d\omega_s\right)\mathbb Q^x(d\omega).}
$$

The integral in its exponent is an [Itô integral](../../../../../../ito-integral.md) under Wiener measure, not an ordinary pathwise line integral. The [Itô formula](../../../../../../ito-s-lemma.md) for $|\omega|^2$ gives

$$
\int_0^t\omega_s\cdot d\omega_s=\frac12\left(|\omega_t|^2-|x|^2-dt\right).
$$

Hence an equivalent endpoint-only Wiener integral is

$$
\boxed{u(t,x)=e^{\lambda(|x|^2+dt)/2}\int e^{-\lambda|\omega_t|^2/2}\,\mathbb Q^x(d\omega).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

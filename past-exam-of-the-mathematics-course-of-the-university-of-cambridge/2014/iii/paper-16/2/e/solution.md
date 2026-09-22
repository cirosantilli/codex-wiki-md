<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Hamiltonian flow](../../../../../../hamiltonian-flow.md) of $H$ solves

$$
\frac d{dt}\phi_H^t(p)=X_H(\phi_H^t(p)),\qquad\phi_H^0(p)=p,
\qquad\iota_{X_H}\omega=dH.
$$

Compactness and the absence of a boundary make this [smooth](../../../../../../smooth-function.md) [vector field](../../../../../../vector-field.md) complete, so the flow exists for all real $t$. The defining equation and [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md) give

$$
\mathcal L_{X_H}\omega=d\iota_{X_H}\omega+\iota_{X_H}d\omega=d^2H=0.
$$

Therefore the [pullback of a differential form](../../../../../../pullback-of-a-differential-form.md) differentiation rule yields

$$
\frac d{dt}(\phi_H^t)^*\omega=(\phi_H^t)^*(\mathcal L_{X_H}\omega)=0,
$$

so $(\phi_H^t)^*\omega=\omega$. Pullback commutes with the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md), and consequently

$$
\boxed{(\phi_H^t)^*\left(\frac{\omega^n}{n!}\right)=\frac{\omega^n}{n!}.}
$$

Thus the flow preserves the [symplectic volume](../../../../../../symplectic-volume.md), in fact the entire [symplectic form](../../../../../../symplectic-form.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

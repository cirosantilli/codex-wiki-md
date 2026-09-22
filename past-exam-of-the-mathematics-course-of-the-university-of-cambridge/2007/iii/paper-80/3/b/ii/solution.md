<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Inverse [Fourier transform](../../../../../../../fourier-transform.md) of the [expected value](../../../../../../../expected-value.md) gives

$$
\boxed{\langle E(x,z)\rangle=e^{i\mu-\sigma^2/2}},
$$

independent of both coordinates. Its squared [modulus](../../../../../../../modulus.md) is the coherent [scalar wave intensity](../../../../../../../scalar-wave-intensity.md) $e^{-\sigma^2}$, which must not be confused with the [mean wave intensity](../../../../../../../ensemble-averaged-wave-intensity.md).

For the latter use the stationary two-point statistics. Let $F_0(d\nu)$ be the uncentered [spectral measure of a stationary random field](../../../../../../../spectral-measure-of-a-stationary-random-field.md) of $E(0,z)$, normalized by

$$
\langle E(0,z+\zeta)E(0,z)^*\rangle=\int e^{i\nu\zeta}F_0(d\nu).
$$

Since $|E(0,z)|=1$, its total mass is $\int F_0(d\nu)=1$. Under free [paraxial propagation](../../../../../../../paraxial-approximation.md) each spectral component is multiplied by $e^{-i\nu^2x/(2k)}$; in its [wave-field correlation](../../../../../../../uncentered-wave-field-correlation.md) this [wave phase](../../../../../../../phase-waves.md) multiplies its [complex conjugate](../../../../../../../complex-conjugate.md) and cancels. The [stationary intensity under free paraxial propagation](../../../../../../../stationary-intensity-under-free-paraxial-propagation.md) is consequently

$$
\boxed{\langle I(x,z)\rangle=\int F_0(d\nu)=1}.
$$

[Stationarity](../../../../../../../stationary-process.md) is essential to this pointwise statement: it makes the spectral covariance diagonal. Conservation of integrated power alone would not show that a particular spatial point keeps the same [scalar wave intensity](../../../../../../../scalar-wave-intensity.md).

The same result follows locally from $I_x+J_z=0$, where $J=\operatorname{Im}(E^*E_z)/k$. Taking [expectations](../../../../../../../expected-value.md) makes $\langle J\rangle$ independent of $z$, so $\partial_x\langle I\rangle=0$. Thus coherent [scalar wave intensity](../../../../../../../scalar-wave-intensity.md) and [mean wave intensity](../../../../../../../ensemble-averaged-wave-intensity.md) are both constant in propagation, with different values. The incoherent contribution has mean $1-e^{-\sigma^2}$. Individual realizations can show focusing and changing [scalar wave intensity](../../../../../../../scalar-wave-intensity.md) even though the [expected value](../../../../../../../expected-value.md) remains constant. All these propagation statements concern the free [parabolic wave equation](../../../../../../../parabolic-wave-equation.md) from part (a).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 80](../../../../paper-80-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

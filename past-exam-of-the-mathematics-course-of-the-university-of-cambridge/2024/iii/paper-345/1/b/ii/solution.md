<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set

$$
s=\phi_1+\phi_2,
\qquad
c=\frac{\phi_1}{s},
$$

where $s>0$. Applying [first-order perturbation of a simple eigenvalue](../../../../../../../first-order-perturbation-of-a-simple-eigenvalue.md) to the [flux Jacobian](../../../../../../../flux-jacobian.md), or expanding its quadratic formula directly, separates the characteristic that changes total concentration from the characteristic that changes composition:

$$
\lambda_s
=\widehat W(1-2s)\bigl[1-\epsilon(2c-1)\bigr]+O(\epsilon^2),
$$



$$
\lambda_c
=\widehat W\bigl[1-s+\epsilon(2c-1)(1+s)\bigr]+O(\epsilon^2).
$$

At $\epsilon=0$, both species move with the common hindered velocity $\widehat W(1-s)$. Summing their conservation laws gives

$$
s_t+\widehat W\,\partial_z\bigl[s(1-s)\bigr]=0,
$$

so the total concentration is a nonlinear [kinematic wave](../../../../../../../kinematic-wave.md):

$$
\frac{dz}{dt}=\widehat W(1-2s),
\qquad
\frac{ds}{dt}=0.
$$

Taking the ratio $c=\phi_1/s$ instead gives the [composition wave in a bidisperse suspension](../../../../../../../composition-wave-in-a-bidisperse-suspension.md)

$$
c_t+\widehat W(1-s)c_z=0,
$$

and hence

$$
\frac{dz}{dt}=\widehat W(1-s),
\qquad
\frac{dc}{dt}=0.
$$

These are the requested leading-order [ordinary differential equations](../../../../../../../ordinary-differential-equation.md) along the two characteristic families.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 345](../../../../paper-345-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

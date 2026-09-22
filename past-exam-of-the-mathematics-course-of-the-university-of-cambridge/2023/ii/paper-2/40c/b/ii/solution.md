<h1 id="40c/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Average the instantaneous [elastic-wave energy flux](../../../../../../../elastic-wave-energy-flux.md) over one temporal period at fixed position. For complex amplitudes,

$$
\langle P_z\rangle
=-\frac12\operatorname{Re}
\left(\widehat\sigma_{zj}\widehat{\dot u}_j^*\right).
$$

Write the evanescent P displacement amplitude as

$$
\widehat{\mathbf u}
=T\mathbf p\,e^{ik_Psx+k_Pqz},
\qquad
\mathbf p=(s,0,-iq),
\qquad
\mathbf p\mathbin{\cdot}\mathbf p=s^2-q^2=1.
$$

For an [isotropic linear elastic material](../../../../../../../linear-elasticity.md) with [Lamé parameters](../../../../../../../lame-parameter.md) $\lambda,\mu$, its stress and velocity amplitudes are

$$
\widehat{\boldsymbol\sigma}
=ik_PT\left(\lambda\mathbf I+2\mu\mathbf p\mathbf p\right)
 e^{ik_Psx+k_Pqz},
\qquad
\widehat{\dot{\mathbf u}}=-i\omega\widehat{\mathbf u}.
$$

Apart from a real common factor,

$$
\widehat\sigma_{zj}\widehat{\dot u}_j^*
\propto
\lambda p_z^*+2\mu p_z(\mathbf p\mathbin{\cdot}\mathbf p^*)
=iq\left[\lambda-2\mu(s^2+q^2)\right],
$$

which is purely imaginary. Its real part vanishes, and hence

$$
\boxed{\langle P_z\rangle=0}.
$$

The converted P-wave is a reactive near-boundary field and transports no time-averaged acoustic energy in the normal direction.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [40C](../../../40c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

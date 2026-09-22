<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [Minkowski metric](../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$ and the convention $S_{fi}=\delta_{fi}+i(2\pi)^4\delta^{(4)}(p_f-p_i)\mathcal M_{fi}$. Put $m=m_t$, $y=\lambda_t/\sqrt2$, $Q=e_t=2/3$ and

$$
D_0=l^2-m^2+i0,\qquad D_1=(l+p_1)^2-m^2+i0,\qquad D_2=(l-p_2)^2-m^2+i0.
$$

The [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) is understood in subsequent denominators. Contracting the [spinor](../../../../spinor.md) indices around the [fermion loop](../../../../fermion-loop.md) gives the [trace](../../../../matrix-trace.md)

$$
T_{\mu\nu}(l)=\operatorname{tr}\!\left[\gamma_\mu(\not l+m)\gamma_\nu(\not l-\not p_2+m)(\not l+\not p_1+m)\right].
$$

Here $\not p=\gamma^\rho p_\rho$ is [Feynman slash notation](../../../../feynman-slash-notation.md). The [closed fermion loop sign](../../../../closed-fermion-loop-sign.md) is $-1$, the three [interaction vertices](../../../../interaction-vertex.md) contribute $(-iy)(-ieQ)^2$, and the three [Dirac propagators](../../../../dirac-propagator.md) contribute $i^3$. Their product, including the [color charge](../../../../color-charge.md) trace, is $-N_cye^2Q^2$. Thus one ordering has

$$
i\mathcal M^{(1)}_{\mu\nu}=-N_cye^2Q^2\int\frac{d^4l}{(2\pi)^4}\frac{T_{\mu\nu}(l)}{D_0D_1D_2},\qquad
\boxed{\mathcal M^{(1)}_{\mu\nu}=iN_cye^2Q^2\int\frac{d^4l}{(2\pi)^4}\frac{T_{\mu\nu}(l)}{D_0D_1D_2}.}
$$

Multiplying by the incoming [polarization vectors](../../../../polarization-vector.md) and adding the exchanged [Feynman diagram](../../../../feynman-diagram.md) gives

$$
\boxed{\mathcal M=\epsilon_1^\mu\epsilon_2^\nu\left[\mathcal M^{(1)}_{\mu\nu}(p_1,p_2)+\mathcal M^{(1)}_{\nu\mu}(p_2,p_1)\right].}
$$

The displayed four-dimensional [Feynman integral](../../../../feynman-integral.md) is formal until regularized; subsequent manipulations use [dimensional regularization](../../../../dimensional-regularization.md), which permits the required [loop momentum](../../../../loop-momentum.md) shifts.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory course of the University of Oxford](../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

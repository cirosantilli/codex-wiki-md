<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After [integration by parts](../../../../integration-by-parts.md), the quadratic [Proca action](../../../../proca-action.md) with an external source is

$$
S[A,J]=\frac12\int d^4x\,A_\mu K^{\mu\nu}A_\nu+\int d^4x\,J^\mu A_\mu,\qquad
K^{\mu\nu}=g^{\mu\nu}(\partial^2+M^2)-\partial^\mu\partial^\nu.
$$

Since $M>0$, this kernel is invertible with the [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md); the massless [gauge redundancy](../../../../gauge-redundancy.md) is absent in this [unitary gauge](../../../../unitary-gauge.md) quadratic action. Complete the square by $A\mapsto A+K_F^{-1}J$ in the [Gaussian functional integral](../../../../gaussian-functional-integral.md). Its source-independent determinant cancels in the normalized [generating functional](../../../../generating-functional.md):

$$
\boxed{\frac{Z[J]}{Z[0]}=\exp\left[-\frac i2\int d^4x\,d^4y\,J_\mu(x)(K_F^{-1})^{\mu\nu}(x-y)J_\nu(y)\right].}
$$

In [Fourier space](../../../../fourier-space.md), the kernel is

$$
K^{\mu\nu}(k)=(M^2-k^2)g^{\mu\nu}+k^\mu k^\nu.
$$

For $k^2\ne0$, use the [transverse projector of a vector field](../../../../transverse-projector-of-a-vector-field.md) $P_T^{\mu\nu}=g^{\mu\nu}-k^\mu k^\nu/k^2$ and the [longitudinal projector of a vector field](../../../../longitudinal-projector-of-a-vector-field.md) $P_L^{\mu\nu}=k^\mu k^\nu/k^2$. Their mixed-index products obey $P_TP_L=0$, so

$$
K=(M^2-k^2)P_T+M^2P_L,\qquad
K^{-1}=\frac{P_T}{M^2-k^2}+\frac{P_L}{M^2}=-\frac{g^{\mu\nu}-k^\mu k^\nu/M^2}{k^2-M^2}.
$$

The last expression also extends to $k^2=0$; that point only obstructs the intermediate projector decomposition. Two source [functional derivatives](../../../../functional-derivative.md) yield the [gauge-boson propagator](../../../../gauge-boson-propagator.md) $D_F=iK_F^{-1}$:

$$
\boxed{D_F^{\mu\nu}(k)=\frac{-i}{k^2-M^2+i0}\left(g^{\mu\nu}-\frac{k^\mu k^\nu}{M^2}\right),\qquad
\langle T A^\mu(x)A^\nu(y)\rangle=\int\frac{d^4k}{(2\pi)^4}e^{-ik\cdot(x-y)}D_F^{\mu\nu}(k).}
$$

The pole residue is the physical massive-vector [massive vector polarization sum](../../../../polarization-sum-for-a-massive-vector-boson.md). The longitudinal term is essential for inverting the quadratic kernel, and makes the naive $M\to0$ limit of this [unitary gauge](../../../../unitary-gauge.md) [Proca propagator](../../../../proca-propagator.md) singular.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

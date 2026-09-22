<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The source uses the forward Fourier phase $e^{ikx}$, so $\widehat{\partial_x A}=-ik\widehat A$. For a nonzero [wavenumber](../../../../../wavenumber.md) put $q=|k|$. Biharmonicity becomes $(\partial_y^2-q^2)^2\widehat A=0$. The decaying solutions are $(C+Dy)e^{-qy}$. The normal-[stress](../../../../../stress.md) condition gives $-k^2\widehat A(k,0)=-\widehat P(k)$, hence $C=\widehat P/k^2$. The shear condition gives $\widehat A_y(k,0)=0$, so $D=qC$. Consequently

$$
\boxed{\widehat A(k,y)=\frac{1+qy}{k^2}\widehat P(k)e^{-qy},\qquad k\ne0.}
$$

Its second derivatives are $\widehat{A_{xx}}=-\widehat P(1+qy)e^{-qy}$ and $\widehat{A_{yy}}=\widehat P(qy-1)e^{-qy}$. The given [strain](../../../../../strain.md)/[stress](../../../../../stress.md) inversion therefore yields

$$
2\mu\widehat v_y=\widehat P(2\nu-1-qy)e^{-qy}.
$$

Integrating in $y$ with the stated decaying-mode condition gives

$$
\boxed{2\mu\widehat v=\left(y+\frac{2(1-\nu)}q\right)\widehat P(k)e^{-qy},\qquad k\ne0.}
$$

This is the [Fourier solution of a loaded elastic half-space](../../../../../fourier-solution-of-a-loaded-elastic-half-space.md).

The zero [wavenumber](../../../../../wavenumber.md) needs separate treatment: these displayed divisions by $k^2$ and $|k|$ are not formulas at $k=0$. In particular a nonzero resultant $\widehat P(0)=\int P\,dx$ is incompatible with an ordinary decaying zero-mode [displacement](../../../../../displacement.md) of the stipulated kind; two-dimensional net loading produces a logarithmic [displacement](../../../../../displacement.md) reference issue. Balanced loads or an appropriate distributional/reference-[displacement](../../../../../displacement.md) formulation are needed for a global transform solution. The nonzero modes and the [displacement](../../../../../displacement.md)-gradient kernel below remain the correct formal calculation; the singular zero mode must not be silently assigned a finite value.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../../split.md)
6. [Elasticity and plasticity course of the University of Oxford](../../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

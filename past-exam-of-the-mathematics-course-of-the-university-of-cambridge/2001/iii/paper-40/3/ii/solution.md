<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The exponent of the point-mass weight is $\beta$, with $0<\beta<1$. At the origin the unreferenced [relative potential](../../../../../../relative-potential.md) has integrand $GBb^{\beta-1}$, whose integral diverges at its upper endpoint. In the origin-referenced potential the two terms cancel pointwise there. More generally, first form their difference at finite cutoffs and then pass to the limit. For any fixed nonzero $(R,z)$, the small-$b$ singular term is $-b^{\beta-1}$, which is integrable because $\beta>0$. At large $b$,

$$
\frac1{\sqrt{R^2+(|z|+b)^2}}-\frac1b
=-\frac{|z|}{b^2}+O(b^{-3}),
$$

so the weighted difference is integrable because $\beta<1$. Hence the referenced potential is well defined, and **its value at the origin is zero**. It is a potential difference for an infinite [astrophysical disk](../../../../../../astrophysical-disk.md), not a potential with zero at infinity. In fact rescaling all lengths shows $\psi_{II}(\lambda R,\lambda z)=\lambda^\beta\psi_{II}(R,z)$; its finite values approach zero at the origin even though its force is singular there.

For $R>0$, differentiation under the convergent force integral in the plane gives

$$
\partial_R\psi_{II}=-GBR\int_0^\infty\frac{b^\beta}{(R^2+b^2)^{3/2}}\,db.
$$

Use $b=R\sqrt{t/(1-t)}$, for which $db=(R/2)t^{-1/2}(1-t)^{-3/2}\,dt$. The powers of $R$, $t$, and $1-t$ then give

$$
\partial_R\psi_{II}=-\frac{GB}{2}R^{\beta-1}\int_0^1t^{(\beta-1)/2}(1-t)^{-\beta/2}\,dt
=\boxed{-CR^{\beta-1}},
$$

where the [Euler beta function](../../../../../../beta-function.md) evaluates the constant as

$$
C=\frac{GB}{2}B\left(\frac{1+\beta}{2},1-\frac\beta2\right)
=\frac{GB}{2}\frac{\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}{\Gamma(3/2)}.
$$

The first [gamma function](../../../../../../gamma-function.md) argument is $(1+\beta)/2$: it follows from adding one to the exponent of $t$. Both [Euler beta function](../../../../../../beta-function.md) arguments are positive in the stated range.

For a [circular orbit](../../../../../../circular-orbit.md) in the plane, $V^2/R=-\partial_R\psi_{II}$. The prescribed [circular speed](../../../../../../circular-speed.md) therefore fixes $C=K^2$ and

$$
B=\frac{2K^2\Gamma(3/2)}{G\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}.
$$

Independently, the [Kuzmin reflection method](../../../../../../kuzmin-reflection-method.md) gives

$$
\Sigma(R)=\frac{B}{2\pi}\int_0^\infty\frac{b^{\beta+1}}{(R^2+b^2)^{3/2}}\,db
=\frac{BR^{\beta-1}}{4\pi}B\left(1+\frac\beta2,\frac{1-\beta}{2}\right).
$$

Here the power of $b$ is one larger than in the force integral, so its [Euler beta function](../../../../../../beta-function.md) arguments differ. Substituting the normalization fixed by the [circular speed](../../../../../../circular-speed.md) yields

$$
\boxed{\Sigma(R)=\frac{K^2}{2\pi G}R^{\beta-1}
\frac{\Gamma(1+\beta/2)\Gamma((1-\beta)/2)}{\Gamma((1+\beta)/2)\Gamma(1-\beta/2)}.}
$$

This [scale-free Kuzmin superposition](../../../../../../scale-free-kuzmin-superposition.md) has nonnegative [surface density](../../../../../../surface-density-of-a-disk.md), finite central enclosed [mass](../../../../../../mass.md), and infinite total [mass](../../../../../../mass.md). Its force and [surface density](../../../../../../surface-density-of-a-disk.md) approach the [Mestel disk](../../../../../../mestel-disk.md) values as $\beta\downarrow0$; that limiting disk requires a different potential reference at the origin.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

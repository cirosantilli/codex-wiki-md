<h1 id="23i/solution">Solution</h1>

↑ **Parent:** [23I](../23i.md)

The [length of a curve](../../../../../length-of-a-curve.md) is $L(\alpha)=\int_a^b\|\alpha'(t)\|dt$. Its [arc length](../../../../../arc-length.md) parameter is $s(t)=\int_a^t\|\alpha'(u)\|du$. Regularity gives $s'(t)>0$, so the inverse function theorem gives a smooth inverse and $\beta(s)=\alpha(t(s))$ has $\|\beta'(s)\|=1$.

Reparametrize a length minimizer to constant speed on $[a,b]$ and use the [energy functional](../../../../../energy-functional.md) $E=\tfrac12\int_a^b\|\alpha'\|^2dt$. By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), every competitor has $E\geq L^2/(2(b-a))$, with equality for constant speed, so this parametrization also minimizes $E$. For a fixed-endpoint [variation](../../../../../variation.md) with tangential [vector field](../../../../../vector-field.md) $V$, differentiation and [integration by parts](../../../../../integration-by-parts.md) give

$$
 \delta E=\int_a^b\langle\alpha',V'\rangle dt
 =-\int_a^b\langle\alpha'',V\rangle dt
 =-\int_a^b\langle\nabla_t\alpha',V\rangle dt.
$$

The boundary term is zero. Arbitrary smooth tangential $V$ of [compact](../../../../../compact-space.md) interior support are realizable by the stated [variation](../../../../../variation.md) fact. Taking $V$ to be a nonnegative cutoff times $\nabla_t\alpha'$ proves $\nabla_t\alpha'=0$. Hence **a length minimizer is a [geodesic](../../../../../geodesic.md) after constant-speed reparametrization**. The original parameter need not be affine: arbitrary varying-speed parametrizations preserve length but have nonzero covariant [acceleration](../../../../../acceleration.md). This qualification is necessary for the literal wording.

For distinct nonantipodal $p,q$ on the punctured unit [sphere](../../../../../sphere.md), there is a unique shorter [great circle](../../../../../great-circle.md) arc, of length $d=\arccos(p\cdot q)<\pi$. A minimizing [curve](../../../../../curve.md) exists **exactly when that shorter arc avoids the removed north pole**. If it avoids the pole it attains the spherical lower bound. If it passes through the pole, arbitrarily small smooth detours have lengths tending to $d$, but equality would force the unique shorter arc, which is unavailable. Thus the infimum is not attained; the longer [great circle](../../../../../great-circle.md) arc is not a substitute minimizer.

For antipodal $p,q$ in the punctured [sphere](../../../../../sphere.md), one can choose a [great circle](../../../../../great-circle.md) semicircle avoiding the north pole; it attains length $\pi$. Thus **every admissible antipodal pair has a minimizer**. If identical endpoints are included despite the earlier distinctness stipulation, the infimum is zero, but no smooth regular [curve](../../../../../curve.md) attains it; only a nonregular constant [curve](../../../../../curve.md) does.

## ↑ Ancestors (10)

1. [23I](../23i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

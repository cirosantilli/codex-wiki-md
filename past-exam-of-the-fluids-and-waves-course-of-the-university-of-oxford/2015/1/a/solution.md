<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the planar [velocity field](../../../../velocity-field.md) as $\mathbf u=(u,v,0)$, with $\mathbf k=(0,0,1)$. Expanding the [curl](../../../../curl.md) gives

$$
\mathbf u=\nabla\times(\psi\mathbf k)=(\psi_y,-\psi_x,0),
\qquad \nabla\psi=\mathbf k\times\mathbf u=(-v,u,0).
$$

Consequently, for a piecewise smooth path $\gamma$ from the origin to $\mathbf x=(x,y)$,

$$
\boxed{\psi(\mathbf x)=\psi(\mathbf0)+\int_\gamma(\mathbf k\times\mathbf u)\cdot d\mathbf r
=\psi(\mathbf0)+\int_\gamma(u\,dy-v\,dx).}
$$

The arbitrary additive constant $\psi(\mathbf0)$ may be set to zero. The integrand is exactly $\nabla\psi\cdot d\mathbf r$, so the [fundamental theorem for line integrals](../../../../fundamental-theorem-for-line-integrals.md) proves [path independence](../../../../path-independence.md) immediately: the difference between two paths is the [line integral](../../../../line-integral.md) of a [gradient](../../../../gradient.md) around a [closed curve](../../../../closed-curve.md), which is zero.

One can also see the local integrability condition from [Green's theorem](../../../../green-theorem.md):

$$
\oint(u\,dy-v\,dx)=\iint(u_x+v_y)\,dx\,dy=0,
$$

because the given representation enforces [incompressibility](../../../../incompressible-flow.md). This second proof applies whenever the region between the paths lies in the regular fluid domain. The question already assumes a globally defined [streamfunction](../../../../stream-function.md); without that assumption, [incompressibility](../../../../incompressible-flow.md) alone would guarantee a global [streamfunction](../../../../stream-function.md) on a [simply connected domain](../../../../simply-connected-domain.md), but a hole carrying nonzero [volume flux](../../../../volumetric-flow-rate.md) could obstruct it.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

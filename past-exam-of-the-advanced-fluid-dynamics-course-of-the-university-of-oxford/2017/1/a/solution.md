<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose two independent labels for the [magnetic field lines](../../../../magnetic-field-line.md), constant along each line. These are [Euler potentials](../../../../euler-potentials.md): $\mathbf B\cdot\nabla\alpha=\mathbf B\cdot\nabla\beta=0$. Where the two [gradients](../../../../gradient.md) are independent, the vector [perpendicular](../../../../orthogonal-vectors.md) to both is $\nabla\alpha\times\nabla\beta$, so initially write

$$
\mathbf B=f\,\nabla\alpha\times\nabla\beta.
$$

The [solenoidal condition](../../../../solenoidal-vector-field.md) gives $0=\nabla\cdot\mathbf B=(\nabla\alpha\times\nabla\beta)\cdot\nabla f$. Thus $f$ is constant along a [field line](../../../../magnetic-field-line.md) and is locally a function of its labels. Redefining one label, for example $\widetilde\beta(\alpha,\beta)=\int^\beta f(\alpha,b)\,db$, absorbs this factor. Dropping the tilde gives

$$
\boxed{\mathbf B=\nabla\alpha\times\nabla\beta.}
$$

This representation automatically has zero [divergence](../../../../divergence.md), since it is also $\nabla\times(\alpha\nabla\beta)$.

For an [magnetic arcade](../../../../magnetic-arcade.md), assign the labels on one polarity of the footpoint surface and transport them along each line to its other footpoint. They specify both line identity and [magnetic flux](../../../../magnetic-flux.md): on a transverse surface, flux coordinates can be chosen so that the [directed flux](../../../../magnetic-flux.md) element is $d\alpha\,d\beta$. In particular,

$$
B_z(x,y,0)=\partial_x\alpha_0\,\partial_y\beta_0-
\partial_y\alpha_0\,\partial_x\beta_0.
$$

The [boundary labels](../../../../euler-potentials.md) at paired footpoints must agree, so prescribed [boundary functions](../../../../boundary-condition.md) encode a compatible [footpoint mapping](../../../../magnetic-field-line.md), not independently arbitrary values at the two ends.

The construction assumes a smooth family of nonintersecting lines that can be labelled from a transverse boundary patch, with suitable patches at nulls or coordinate singularities. A local [Euler-potential representation](../../../../euler-potentials.md) does not establish the existence of two globally single-valued regular labels for every possible [solenoidal field](../../../../solenoidal-vector-field.md); closed, recurrent or more complicated [field topology](../../../../magnetic-field-line.md) can obstruct such a global choice. The line-tied [magnetic arcade](../../../../magnetic-arcade.md) geometry supplies the relevant simplifying assumption here.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

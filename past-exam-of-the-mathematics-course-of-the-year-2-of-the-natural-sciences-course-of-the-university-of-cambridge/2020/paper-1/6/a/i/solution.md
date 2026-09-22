<h1 id="6/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

When $r=p'$, write the differential expression in divergence form,

$$
\widetilde L y=(py')'+qy.
$$

Two integrations by parts give the [Lagrange identity for a Sturm-Liouville operator](../../../../../../lagrange-identity-for-a-sturm-liouville-operator.md):

$$
\langle f,\widetilde Lg\rangle-\langle\widetilde Lf,g\rangle
=\left[p(fg'-f'g)\right]_a^b.
$$

The $q$ terms cancel because $q$ is real. Hence the exact boundary criterion, in the sense of [self-adjointness](../../../../../../self-adjoint-operator.md) defined in the question, is

$$
\boxed{\left[p(fg'-f'g)\right]_a^b=0\quad\text{for every admissible pair }f,g.}
$$

At regular endpoints, all separated homogeneous conditions of the following type satisfy it:

$$
\alpha_a y(a)+\beta_a p(a)y'(a)=0,\qquad
\alpha_b y(b)+\beta_b p(b)y'(b)=0,
$$

with real coefficients, not both zero at either endpoint. The allowed value-and-flux pairs at an endpoint are proportional, so their [determinant](../../../../../../determinant.md) $p(fg'-f'g)$ vanishes. This includes [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md), [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md), [Robin boundary conditions](../../../../../../robin-boundary-condition.md) and arbitrary mixtures of these at the two ends.

Coupled conditions can also work: periodic conditions $y(b)=y(a)$ and $p(b)y'(b)=p(a)y'(a)$ make the two endpoint expressions equal; simultaneous minus signs give the antiperiodic case. Thus requiring each endpoint term separately to vanish is sufficient, but not necessary.

More generally, for regular endpoints set $Y=(y(a),y(b))^{\mathsf T}$ and $N=(-p(a)y'(a),p(b)y'(b))^{\mathsf T}$. All maximal homogeneous self-adjoint [boundary conditions](../../../../../../boundary-condition.md) can be written $AY+BN=0$ with real two-by-two [matrices](../../../../../../matrix.md) satisfying $\operatorname{rank}(A\ B)=2$ and $AB^{\mathsf T}=BA^{\mathsf T}$. If an endpoint is singular, the relevant limiting boundary form and admissible domain must instead be specified; the assumption $p>0$ only in the interior does not itself fix those endpoint limits.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

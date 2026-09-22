<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V(\phi)=m^2\phi^2/2+\lambda(\phi^2)^2/4$, where $\phi^2=\sum_i\phi_i^2$. Its stationary-point equation is $(m^2+\lambda\phi^2)\phi_i=0$.

For $m^2>0$, the unique minimum is $\phi=0$. The quadratic [mass term](../../../../../../mass-term.md) is $m^2\delta_{ij}$, so **there are $n$ [real scalar fields](../../../../../../real-scalar-field.md), all of mass $\sqrt{m^2}$**, and the global [special orthogonal group](../../../../../../special-orthogonal-group.md) $SO(n)$ remains unbroken.

For $m^2<0$, write $v^2=-m^2/\lambda$. The [vacuum manifold](../../../../../../vacuum-manifold.md) is the sphere $\phi^2=v^2$. Choose $\langle\phi\rangle=v e_n$. The transformations preserving this [vacuum expectation value](../../../../../../vacuum-expectation-value.md) rotate the first $n-1$ components, giving **$SO(n)\to SO(n-1)$**. At this vacuum the potential's [Hessian matrix](../../../../../../hessian-matrix.md) is

$$
\left.\frac{\partial^2V}{\partial\phi_i\partial\phi_j}\right|_{ve_n}
=2\lambda v^2\delta_{in}\delta_{jn}.
$$

Writing $\phi=(\pi_1,\ldots,\pi_{n-1},v+\eta)$, the radial mode $\eta$ therefore has

$$
\boxed{m_\eta^2=2\lambda v^2=-2m^2,\qquad m_{\pi_a}^2=0\quad(a=1,\ldots,n-1).}
$$

These are one massive radial scalar and $n-1$ physical [Goldstone bosons](../../../../../../goldstone-boson.md). The [Goldstone theorem](../../../../../../goldstone-theorem.md) applies to the broken global generators; the flat angular directions of the [vacuum manifold](../../../../../../vacuum-manifold.md) explain their zero masses. The [spontaneous symmetry breaking](../../../../../../spontaneous-symmetry-breaking.md) is a choice of vacuum, not a change in the invariant Lagrangian. For $n=1$ there are no continuous angular directions: only the radial scalar remains, and the potential's discrete $\phi\mapsto-\phi$ symmetry is broken.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

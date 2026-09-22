<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

In vacuum [magnetostatics](../../../../../magnetostatics.md), the two relevant [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\cdot\mathbf B=0,\qquad \nabla\times\mathbf B=\mu_0\mathbf J.
$$

Orient the unit normal $\mathbf n$ from the minus side to the plus side. Integrating [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) over a pillbox straddling the [current sheet](../../../../../current-sheet.md) and shrinking its thickness gives $\mathbf n\cdot(\mathbf B_+-\mathbf B_-)=0$.

To obtain the tangential condition, choose an arbitrary tangent unit vector $\mathbf t$ and an infinitesimal rectangle with its long sides of length $\ell$ parallel to $\mathbf t$ on the two sides of the sheet. Orient its surface normal as $\mathbf n\times\mathbf t$, so that its plus-side long edge is traversed along $\mathbf t$. The line [integral](../../../../../integral.md) in [Ampère's law](../../../../../ampere-s-circuital-law.md) tends to $\ell\mathbf t\cdot(\mathbf B_+-\mathbf B_-)$. The enclosed [electric current](../../../../../electric-current.md) tends to $\ell\mathbf s\cdot(\mathbf n\times\mathbf t)$. Hence

$$
\mathbf t\cdot(\mathbf B_+-\mathbf B_-)=\mu_0\mathbf t\cdot(\mathbf s\times\mathbf n).
$$

Because this holds for every tangent direction and the normal jump is zero,

$$
\boxed{\mathbf n\times(\mathbf B_+-\mathbf B_-)=\mu_0\mathbf s.}
$$

Here $\mathbf s\cdot\mathbf n=0$, as required for a [surface current density](../../../../../surface-current-density.md).

The [force on a current sheet from the mean magnetic field](../../../../../force-on-a-current-sheet-from-the-mean-magnetic-field.md) is

$$
\boxed{\mathbf f_S=\mathbf s\times\frac{\mathbf B_++\mathbf B_-}{2}.}
$$

The mean removes the sheet's equal and opposite local self-fields, leaving the field that acts on its current through the [Lorentz force](../../../../../lorentz-force.md). Using a one-sided limiting [magnetic field](../../../../../magnetic-field.md) would incorrectly include the sheet's own force.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

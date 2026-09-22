<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

An [exact differential](../../../../../exact-differential.md) is a one-form equal to $d\Phi$ for a single-valued scalar function $\Phi$ on the domain. In Euclidean coordinates this means its vector coefficients form $\nabla\Phi$. Integrating the first component of $F$ with respect to $x$, then matching the other components, gives

$$
\boxed{\Phi(x,y,z)=z^3(e^x-e^y)+x^3(e^y-e^z)+C.}
$$

Differentiating checks all three components. Since the domain $\mathbb R^3$ is connected, two such potentials differ only by a constant, so this is the most general potential.

At both specified endpoints the nonconstant terms vanish. The [fundamental theorem for line integrals](../../../../../fundamental-theorem-for-line-integrals.md) gives **zero for the line integral along every path joining the two points**.

For the planar field, choose a continuous lift $\theta(t)$ of the polar angle along a curve avoiding the origin. Differentiating the angle gives

$$
G\cdot dx=\frac{-y\,dx+x\,dy}{x^2+y^2}=d\theta.
$$

On the closed curve the angle increases by $2\pi$ times its [winding number](../../../../../winding-number.md). Thus

$$
\boxed{\oint_CG\cdot dx=2\pi.}
$$

The angle differential is locally exact but not globally exact on the [punctured plane](../../../../../punctured-complex-plane.md): the angle lift need not return to its initial value. This is the [nonexact angular one-form](../../../../../nonexact-angular-one-form.md), whose nonzero closed-path integral obstructs a global potential.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

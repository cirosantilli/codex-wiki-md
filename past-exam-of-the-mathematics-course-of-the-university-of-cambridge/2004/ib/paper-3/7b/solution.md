<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Choose positive circulation anticlockwise as viewed from positive $z$. The linked magnetic flux is $\Phi=2\ell XB$, so [Faraday law](../../../../../faraday-s-law-of-induction.md), including the motional contribution, gives

$$
\boxed{\mathcal E=-\frac{d\Phi}{dt}=-2\ell\frac{d(XB)}{dt}.}
$$

The conducting circuit consists of two arms of length $X$ and two transverse pieces of length $2\ell$. Its resistance is $\mathcal R=2R(X+2\ell)$, where $R$ is resistance per unit length. Neglecting self-inductance as in the quasistatic circuit model, the current is

$$
I=\frac{\mathcal E}{\mathcal R}=-\frac{\ell}{R(X+2\ell)}\frac{d(XB)}{dt}.
$$

On the moving rod this positive current points along $+y$, so the [Lorentz force](../../../../../lorentz-force.md) is $I(2\ell\mathbf e_y)\times(B\mathbf e_z)=2\ell IB\mathbf e_x$. Its mass is $2\ell M$, not the mass of the entire circuit. Newton's equation consequently gives

$$
\boxed{M\ddot X=IB=-\frac{B}{R(X+2\ell)}\frac{d(X\ell B)}{dt}.}
$$

For constant $B$, the force opposes $\dot X$, as expected from [Lenz's law](../../../../../lenz-s-law.md). The prescribed time dependence of the external field can also supply energy to the rod.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

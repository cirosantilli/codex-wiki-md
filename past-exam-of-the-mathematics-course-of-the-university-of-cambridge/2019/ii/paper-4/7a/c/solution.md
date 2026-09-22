<h1 id="7a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the argument of $z$ increase by $2\pi$ along a counterclockwise path enclosing both branch points. On a large circle, the branch chosen in part (a) satisfies

$$
\sqrt{1-t^2}\sim-it,
\qquad
\frac1{\sqrt{1-t^2}}\sim\frac{i}{t}.
$$

The change in the primitive is consequently

$$
\lim_{R\to\infty}\oint_{|t|=R}\frac{dt}{\sqrt{1-t^2}}
=\oint\frac{i}{t}\,dt
=-2\pi.
$$

Equivalently, this is the composition of the two reflections described by the [monodromy of the complex inverse sine](../../../../../../monodromy-of-the-complex-inverse-sine.md). Thus, for this orientation,

$$
\boxed{\operatorname{arcsin}(e^{2\pi i}z)=\operatorname{Arcsin}(z)-2\pi.}
$$

The reverse orientation gives $\operatorname{Arcsin}(z)+2\pi$. Both continued values invert the same $z$, so $\sin(w-2\pi)=\sin w$ on an open set of inverse values. The [identity theorem](../../../../../../identity-theorem.md) extends this equality to every $w\in\mathbb C$, proving the [periodicity of the complex sine](../../../../../../periodicity-of-the-complex-sine.md):

$$
\boxed{\sin(w+2\pi)=\sin w.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7A](../../7a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

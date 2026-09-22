<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An element $x$ of a unital [C-star algebra](../../../../../../c-star-algebra.md) is positive when $x=y^*y$ for some $y$, equivalently when $x=x^*$ and $\sigma(x)\subseteq[0,\infty)$. The continuous functional calculus for the nonnegative function $t\mapsto\sqrt t$ defines a positive element $x^{1/2}$ satisfying $(x^{1/2})^2=x$. If a positive $z$ also satisfies $z^2=x$, functional calculus for $z$ gives $z=\sqrt{z^2}=\sqrt x$, proving uniqueness. For a positive operator $T=S^*S$ on $\ell^2$,

$$
\langle T\xi,\xi\rangle=\|S\xi\|^2\geq0.
$$

For arbitrary $T$, put $|T|=(T^*T)^{1/2}$. Then

$$
\||T|\xi\|^2
=\langle T^*T\xi,\xi\rangle
=\|T\xi\|^2,
$$

so $\ker|T|=\ker T$. Define

$$
U_0(|T|\xi)=T\xi
$$

on $\operatorname{im}|T|$. The kernel identity makes this well-defined, and the norm identity makes it an isometry. Extend it continuously to

$$
\overline{\operatorname{im}|T|}=(\ker|T|)^\perp=(\ker T)^\perp
$$

and set it equal to zero on $\ker T$. The resulting $U$ is a [partial isometry](../../../../../../partial-isometry.md), has $\ker U=\ker T$, and satisfies the [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) $T=U|T|$.

Finally $U^*U$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto $(\ker T)^\perp$, which contains the range of $|T|$. Therefore

$$
\boxed{U^*T=U^*U|T|=|T|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

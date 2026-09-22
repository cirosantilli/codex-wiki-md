<h1 id="36b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [source-free Maxwell equations in a linear medium](../../../../../../source-free-maxwell-equations-in-a-linear-medium.md) are

$$
\nabla\cdot D=0,\qquad
\nabla\cdot B=0,
$$



$$
\nabla\times E=-\frac{\partial B}{\partial t},
\qquad
\nabla\times H=\frac{\partial D}{\partial t},
$$

with $D=\epsilon E$ and $B=\mu H$.

Take complex plane waves

$$
E=E_0e^{i(k\cdot x-\omega t)},
\qquad
B=B_0e^{i(k\cdot x-\omega t)}.
$$

The divergence equations give

$$
k\cdot E_0=k\cdot B_0=0,
$$

and [Faraday's law](../../../../../../faraday-s-law-of-induction.md) gives

$$
\boxed{B_0=\frac1\omega k\times E_0}.
$$

Ampère's law gives

$$
k\times\frac{B_0}{\mu}=-\omega\epsilon E_0.
$$

Substituting the expression for $B_0$ and using  
$k\times(k\times E_0)=-|k|^2E_0$ yields

$$
\frac{|k|^2}{\mu\omega}E_0
=\omega\epsilon E_0.
$$

Hence the [plane electromagnetic wave in a linear medium](../../../../../../plane-electromagnetic-wave-in-a-linear-medium.md) has

$$
\boxed{\omega^2=\frac{|k|^2}{\epsilon\mu}},
\qquad
\boxed{v=\frac{\omega}{|k|}
=\frac1{\sqrt{\epsilon\mu}}},
$$

and equivalently

$$
\boxed{B_0=\sqrt{\epsilon\mu}\,\widehat k\times E_0}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [36B](../../36b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

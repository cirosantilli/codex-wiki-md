<h1 id="37a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The spatial part of the [Lorentz force](../../../../../../lorentz-force.md) is

$$
\frac d{dt}(\gamma m\mathbf v)
=q(\mathbf E+\mathbf v\times\mathbf B).
$$

Part (c), together with $\mathcal E=\gamma mc^2$, gives

$$
\frac{d\gamma}{dt}
=\frac q{mc^2}\mathbf E\mathbin{\cdot}\mathbf v.
$$

Writing $\mathbf a=d\mathbf v/dt$ and expanding the momentum derivative,

$$
m\gamma\mathbf a+m\mathbf v\frac{d\gamma}{dt}
=q(\mathbf E+\mathbf v\times\mathbf B).
$$

Substitution of $d\gamma/dt$ gives the [coordinate acceleration of a relativistic charged particle](../../../../../../coordinate-acceleration-of-a-relativistic-charged-particle.md):

$$
\boxed{
\frac{d\mathbf v}{dt}
=\frac q{m\gamma}
\left[
\mathbf E+\mathbf v\times\mathbf B
-\frac1{c^2}\mathbf v(\mathbf v\mathbin{\cdot}\mathbf E)
\right]
}.
$$

In the nonrelativistic limit $|\mathbf v|/c\to0$, one has $\gamma\to1$ and the final term is smaller by order $v^2/c^2$. Hence

$$
\boxed{
m\frac{d\mathbf v}{dt}
=q(\mathbf E+\mathbf v\times\mathbf B)
},
$$

which is precisely Newton's second law with the ordinary Lorentz force.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [37A](../../37a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

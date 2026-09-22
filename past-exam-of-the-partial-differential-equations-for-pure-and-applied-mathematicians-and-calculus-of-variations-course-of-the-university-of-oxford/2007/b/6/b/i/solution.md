<h1 id="b/6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Jacobi equation](../../../../../../jacobi-equation.md) is $z''+\lambda^2z=0$. For $|\lambda|<\pi$ the [function](../../../../../../function-split.md) $z=\cos(\lambda(x-1/2))$ is positive on the closed interval. The preceding square identity gives

$$
I(u)=\int_0^1z^2[(u/z)']^2dx,
$$

with $z=1$ if $\lambda=0$. As in part (a), its positive minimum and bounded derivative provide a constant $\gamma>0$ with $I(u)\geq\gamma\|u\|_{H^1}^2$. The [second variation](../../../../../../second-variation.md) at zero is $2I$, so is positive, and **zero is the unique [global minimizer](../../../../../../global-minimizer.md)**.

For a fixed zero-trace $u$, positivity of $\int u'^2-\lambda^2\int u^2$ for all $\lambda^2<\pi^2$ gives, by letting $\lambda^2\uparrow\pi^2$,

$$
\boxed{\int_0^1u'^2\geq\pi^2\int_0^1u^2.}
$$

This derivation did not assume the sharp inequality in advance. For equality, the nonnegative quadratic form $Q(u)=\int(u'^2-\pi^2u^2)$ has $Q(u)=0$. Expanding $Q(u+t\phi)\geq0$ for both signs of $t$ forces $\int u'\phi'-\pi^2u\phi=0$ for every test. Thus $u''+\pi^2u=0$, and the zero endpoint values give **exactly $u(x)=C\sin(\pi x)$**, including $C=0$. These [functions](../../../../../../function-split.md) do give equality.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

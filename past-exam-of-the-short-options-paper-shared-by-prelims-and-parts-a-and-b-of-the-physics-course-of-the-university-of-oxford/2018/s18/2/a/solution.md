<h1 id="s18/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x_<=\min(x,x')$ and $x_>=\max(x,x')$. A homogeneous solution vanishing at the left wall is $u(x)=\sin[k(x+a/2)]$; one vanishing at the right wall is $v(x)=\sin[k(a/2-x)]$. Their [Wronskian](../../../../../wronskian.md) is $uv'-u'v=-k\sin ka$. Continuity and the source [derivative](../../../../../derivative.md) jump $G'_+-G'_-=-2m/\hbar^2$ therefore give

$$
\boxed{G(x,x')=\frac{2m}{k\hbar^2\sin ka}
\sin[k(x_<+a/2)]\sin[k(a/2-x_>)].}
$$

This is exactly the printed form because $x_<= (x+x'-|x-x'|)/2$ and $x_>= (x+x'+|x-x'|)/2$, with a minus sign from reversing the argument of the second [sine](../../../../../sine.md).

The true poles occur at $k_n=n\pi/a$, $n=1,2,\ldots$, corresponding to

$$
\boxed{E_n=\frac{\hbar^2\pi^2n^2}{2ma^2}.}
$$

The apparent zero at $k=0$ is removable: the numerator and $k\sin ka$ both vanish quadratically. Negative values of $k_n$ duplicate the same energies, rather than describing extra levels. The [boundary conditions](../../../../../boundary-condition.md) and source jump uniquely determine the inverse whenever $E$ is not an [eigenvalue](../../../../../eigenvalue.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The printed hint with unchanged $\sigma$ is not a valid [change of variables](../../../../../../change-of-variables-formula.md): at fixed $\sigma$, the outgoing velocities forget the direction of $v-v_*$. A correct proof uses the [angular exchange for elastic collisions](../../../../../../angular-exchange-for-elastic-collisions.md).

Set $C=(v+v_*)/2$ and $v-v_*=r\omega$, where $r>0$ and $\omega\in\mathbb S^2$. Then $dv\,dv_*=dC\,r^2dr\,d\omega$, while $v'=C+r\sigma/2$ and $v_*'=C-r\sigma/2$. The gain [integral](../../../../../../integral.md) becomes

$$
\int f(C+r\sigma/2)f(C-r\sigma/2)e^{-i(C+r\omega/2)\cdot\xi}
\,dC\,r^2dr\,d\omega\,d\sigma.
$$

Exchange the two independently integrated angular variables $\omega$ and $\sigma$. The measure is unchanged, and reverting to $v=C+r\omega/2$, $v_*=C-r\omega/2$ gives

$$
\boxed{\int f(v')f(v_*')e^{-iv\cdot\xi}\,dv\,dv_*\,d\sigma
=\int f(v)f(v_*)e^{-i(v+v_*)\cdot\xi/2}e^{-i|v-v_*|\sigma\cdot\xi/2}\,dv\,dv_*\,d\sigma}.
$$

The measure-zero set $r=0$ causes no difficulty. This proves the requested identity without invoking the false fixed-$\sigma$ Jacobian assertion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

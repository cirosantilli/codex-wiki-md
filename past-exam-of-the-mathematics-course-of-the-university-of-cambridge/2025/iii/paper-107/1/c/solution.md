<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a closed ball $\overline{B_R(a)}\subset\Omega$, and let $v$ solve the [Dirichlet problem](../../../../../../dirichlet-problem.md) for the [Laplace equation](../../../../../../laplace-equation.md) in this ball with boundary data $u$. Put $w=u-v$. The function $w$ is continuous, vanishes on the boundary, and inherits the restricted spherical mean identity because $v$ has the full [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md).

Suppose $M=\max_{\overline{B_R(a)}}w>0$. Its maximum set $E$ is a nonempty compact subset of the open ball. Choose $x\in E$ maximizing $|x-a|$. For every sufficiently small radius in the sequence attached to $x$,

$$
M=w(x)=\frac1{|\partial B_r|}\int_{\partial B_r(x)}w\leq M.
$$

Equality of the average with the maximum and [continuity](../../../../../../continuous-function.md) imply that the whole sphere belongs to $E$. Its point in the direction from $a$ through $x$ lies farther from $a$ than $x$ does; if $x=a$, any point on the sphere does. Both cases contradict the choice of $x$. Hence $w\leq0$, and applying the same argument to $-w$ gives $w=0$.

**Thus $u=v$ on every relatively compact ball. It is consequently harmonic and smooth locally, proving the [local converse to the mean value property](../../../../../../local-converse-to-the-mean-value-property.md).**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M=\max_Su$ and suppose $u(z_0)=M$. The sub-mean inequality on every closed disk contained in $S$ gives

$$
M=u(z_0)\leq\frac1{2\pi}\int_0^{2\pi}
u(z_0+re^{i\theta})\,d\theta\leq M.
$$

Equality holds throughout. If $u$ were strictly below $M$ at one point of the circle, upper semicontinuity would make it uniformly below $M$ on a small arc, contradicting equality of the average. Thus $u=M$ on every sufficiently small circle centered at $z_0$, and hence throughout a neighborhood of $z_0$.

The set $\{u=M\}$ is therefore open. It is also closed because upper semicontinuity makes $\{u<M\}$ open. Since the domain is connected and $\{u=M\}$ is nonempty, it is all of $S$. This proves the [maximum principle for subharmonic functions](../../../../../../maximum-principle-for-subharmonic-functions.md).

Let

$$
R(z)=(A-zI)^{-1}.
$$

The resolvent set is open, and the [resolvent of an element](../../../../../../resolvent-of-an-element.md) is operator-valued holomorphic on each of its components. Fix $z_0$ in the resolvent set. For any $\delta>0$, choose unit vectors $x,y$ such that

$$
|\langle R(z_0)x,y\rangle|>\|R(z_0)\|-\delta.
$$

The scalar function $f(z)=\langle R(z)x,y\rangle$ is holomorphic. Its modulus is subharmonic, so

$$
\|R(z_0)\|-\delta
<|f(z_0)|
\leq\frac1{2\pi}\int_0^{2\pi}|f(z_0+re^{i\theta})|\,d\theta
\leq\frac1{2\pi}\int_0^{2\pi}\|R(z_0+re^{i\theta})\|\,d\theta.
$$

Letting $\delta\downarrow0$ proves that the [resolvent norm](../../../../../../resolvent-norm.md) is subharmonic on the resolvent component containing $z_0$.

Use the convention that the reciprocal resolvent norm is zero on the spectrum. Suppose a bounded component $U$ of

$$
\{z:\|R(z)\|^{-1}<\epsilon\}
$$

contained no spectral point. A spectral point in its boundary would belong to the same pseudospectral component, so $\overline U$ is contained in the resolvent set. On $\partial U$ one has $\|R(z)\|\leq\epsilon^{-1}$, whereas inside $U$ one has $\|R(z)\|>\epsilon^{-1}$. Continuity on the compact set $\overline U$ makes the resolvent norm attain a maximum at an interior point. The subharmonic maximum principle would make it constant, contradicting its boundary values. Hence every bounded component of the [pseudospectrum](../../../../../../pseudospectrum.md) contains spectrum:

$$
\boxed{U\cap\operatorname{Sp}(A)\ne\varnothing}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

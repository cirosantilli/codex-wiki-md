<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the right-[comodule](../../../../../../comodule.md) [braiding](../../../../../../braiding.md) convention in part (a), the defining formula is

$$
C(e_i\otimes e_j)=\sum_{k,l}e_l\otimes e_k\,r(t_{ki},t_{lj}).
$$

Consequently the scalar form on generators is the following table, with row the first argument and column the second:

$$
\boxed{\begin{array}{c|rrrr}
r&a&b&c&d\\\hline
a&q^{1/2}&0&0&q^{-1/2}\\
b&0&0&q^{-1/2}(q-q^{-1})&0\\
c&0&0&0&0\\
d&q^{-1/2}&0&0&q^{1/2}
\end{array}.}
$$

For example, the extra $e_2\otimes e_1$ component of $C(e_2\otimes e_1)$ is $r(b,c)=q^{-1/2}(q-q^{-1})$. The other off-diagonal component gives $r(d,a)=q^{-1/2}$.

For arbitrary elements of the [FRT bialgebra](../../../../../../frt-bialgebra.md), extend this table by bilinearity, the unit rule $r(1,z)=r(z,1)=\varepsilon(z)$, and

$$
r(uv,z)=\sum r(u,z_{(1)})r(v,z_{(2)}),\qquad
r(u,vw)=\sum r(u_{(1)},w)r(u_{(2)},v).
$$

These are an explicit recursive algorithm for any two words in the generators, so the table determines the entire [cobraiding](../../../../../../coquasitriangular-structure.md). The braid equation for $C$ ensures the algorithm annihilates the defining coefficient relations in either argument: moving one crossing past two successive crossings gives precisely the two reductions of a quadratic colinearity relation. Thus it descends from the free [algebra over a field](../../../../../../algebra-over-a-field.md) to the [FRT bialgebra](../../../../../../frt-bialgebra.md). For the convolution inverse, use the inverse of $R=\tau C$, where $\tau$ flips the tensor factors: its coefficients are $\bar r(t_{ki},t_{lj})=(R^{-1})_{kl,ij}$. Equivalently, in the flipped coefficient formula use $\tau C^{-1}\tau$, not $C^{-1}$ alone. This gives $\bar r(a,a)=\bar r(d,d)=q^{-1/2}$, $\bar r(a,d)=\bar r(d,a)=q^{1/2}$, $\bar r(b,c)=-q^{1/2}(q-q^{-1})$, and all other generator values zero. This specifies the [coquasitriangular structure](../../../../../../coquasitriangular-structure.md) completely, not just its values on degree-one elements.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

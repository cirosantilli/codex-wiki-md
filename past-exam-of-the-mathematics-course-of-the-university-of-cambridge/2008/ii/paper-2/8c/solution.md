<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

For the [beta function](../../../../../beta-function.md), split $1=t+(1-t)$ inside the integral to obtain $B(z,q)=B(z,q+1)+B(z+1,q)$. Integrating the derivative of $t^q(1-t)^z$ over $(0,1)$ gives $qB(z+1,q)=zB(z,q+1)$, since both endpoint terms vanish in the initial domain. Combining these identities yields

$$
\boxed{B(z,q)=\frac{z+q}{z}B(z+1,q).}
$$

Repeatedly apply this recurrence until $\operatorname{Re}(z+n)>0$. Each resulting expression agrees with the original integral on overlap, so it gives its unique [analytic continuation](../../../../../analytic-continuation.md). Possible singularities are only $z=0,-1,-2,\ldots$.

Near $z=0$, $zB(z,q)\to qB(1,q)=1$. Continuing the recurrence downwards gives

$$
\boxed{\operatorname{Res}_{z=-n}B(z,q)=\frac{(-1)^n}{n!}(q-1)(q-2)\cdots(q-n),\qquad n\ge0,}
$$

where the empty product is $1$. The recurrence shows that each singularity is at most a [simple pole](../../../../../simple-pole.md). If $q$ is not a positive integer, all these residues are nonzero and all the listed points are poles. If $q=m$ is a positive integer, poles occur only for $0\le n<m$; the later candidates are removable, as is also clear from $B(z,m)=(m-1)!/[z(z+1)\cdots(z+m-1)]$. This qualification matters when claiming a pole at every nonpositive integer.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

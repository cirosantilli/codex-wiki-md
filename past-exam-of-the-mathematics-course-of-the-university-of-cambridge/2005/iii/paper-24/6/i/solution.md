<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use cohomological degree, and write the [Sullivan minimal models](../../../../../../sullivan-minimal-model.md) as

$$
M(\mathbb{CP}^n)=(\Lambda(x_2,y_{2n+1}),d),
\qquad dx=0,\quad dy=x^{n+1},
$$

and

$$
M(S^{2n})=(\Lambda(u_{2n},v_{4n-1}),d),
\qquad du=0,\quad dv=u^2.
$$

The subscripts indicate degrees. The even generators generate a [polynomial ring](../../../../../../polynomial-ring.md) and the odd generators an [exterior algebra](../../../../../../exterior-algebra.md). Their [cohomology rings](../../../../../../cohomology-ring.md) are respectively $\mathbb Q[x]/(x^{n+1})$ and $\mathbb Q[u]/(u^2)$, since each odd differential kills exactly the indicated non-zero-divisor polynomial relation. These are the usual projective-space and even-sphere [minimal models](../../../../../../sullivan-minimal-model.md).

Orient the top classes so that the degree-one condition is $f^*[u]=[x^n]$. A representative model map must send $u$ to $x^n$. It must send $v$ to an element of degree $4n-1$ with differential $x^{2n}$. The element $x^{n-1}y$ has exactly these properties. Thus

$$
\boxed{f^*:M(S^{2n})\longrightarrow M(\mathbb{CP}^n),
\qquad u\longmapsto x^n,\quad v\longmapsto x^{n-1}y.}
$$

The differential check is $d(x^{n-1}y)=x^{n-1}x^{n+1}=x^{2n}=(f^*u)^2$. In these degrees there is no other available monomial: even powers of $x$ have even degree, and an odd monomial is a power of $x$ times $y$. Hence the coefficient is forced by the differential. For $n=1$ the two models coincide and the map is the identity model map.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

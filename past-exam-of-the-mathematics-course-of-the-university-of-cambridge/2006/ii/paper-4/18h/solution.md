<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

Take $u\in L\setminus K$, whose [irreducible polynomial](../../../../../irreducible-polynomial.md) is $t^2+ct+d$. Since the characteristic is not two, $x=2u+c$ satisfies $x^2=c^2-4d=a\in K$ and $L=K(x)$. Irreducibility makes $a$ nonzero and nonsquare. If another [quadratic extension](../../../../../quadratic-extension.md) is $K(y)$ with $y^2=b$, an isomorphism sends $x$ to $s+ty$, with $t\ne0$. Squaring gives $a=s^2+t^2b+2sty$. Linear independence of $1,y$ forces $s=0$, so $a=t^2b$ and $b/a$ is a square. Conversely, if $b/a=q^2$, sending $x$ to $y/q$ gives an isomorphism. If $b$ itself is a square, the target is just $K$ and cannot be isomorphic; the square-ratio condition also fails.

The [multiquadratic field](../../../../../multiquadratic-field.md) $F$ is the [splitting field](../../../../../splitting-field.md) of $\prod_i(t^2-a_i)$, a product of separable quadratic polynomials: each has distinct roots because $a_i\ne0$ and the characteristic is not two. Even if factors repeat, this splitting field is a separable normal extension, and therefore Galois. Each automorphism sends $x_i$ to $\pm x_i$, and these signs determine it, embedding its [Galois group](../../../../../galois-group.md) into $(\mathbb Z/2)^n$. Every [subgroup](../../../../../subgroup.md) of this [elementary abelian group](../../../../../elementary-abelian-group.md) is $(\mathbb Z/2)^m$ for some $m\le n$.

For a quadratic intermediate field, its fixing [subgroup](../../../../../subgroup.md) $H$ has index two and is the kernel of a nontrivial [one-dimensional character](../../../../../one-dimensional-character.md) $\chi:G\to\{\pm1\}$. The coordinate sign characters span the dual of $G$: a [linear functional](../../../../../linear-functional.md) on the subspace $G\subseteq\mathbb F_2^n$ extends to the ambient space by extending a basis. Hence $\chi=\prod_{i\in I}\chi_i$ for some subset $I$. Set $y=\prod_{i\in I}x_i$. Then $\sigma(y)=\chi(\sigma)y$, so $y$ is fixed by $H$ but not by all of $G$, and $y^2=\prod_{i\in I}a_i\in K$. Thus $K(y)$ is quadratic and equals the [fixed field](../../../../../fixed-field.md) of $H$. This constructs all [quadratic subfields of a multiquadratic extension](../../../../../quadratic-subfields-of-a-multiquadratic-extension.md):

$$
\boxed{L=K\left(\prod_{i\in I}x_i\right)}.
$$

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

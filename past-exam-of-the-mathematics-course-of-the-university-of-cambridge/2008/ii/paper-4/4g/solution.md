<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

A binary [cyclic code](../../../../../cyclic-code.md) is a linear subspace of $\mathbb F_2^N$ invariant under cyclic coordinate shift. Associate a word $(c_0,\ldots,c_{N-1})$ to $\sum c_jX^j$ in $\mathbb F_2[X]/(X^N-1)$. Cyclic shift is multiplication by $X$, so linearity and shift invariance make the code an ideal of this quotient.

Its inverse image in $\mathbb F_2[X]$ is an ideal containing $(X^N-1)$. Since a [polynomial](../../../../../polynomial-split.md) ring over a field is a [principal ideal domain](../../../../../principal-ideal-domain.md), that inverse image is $(g)$ for a unique monic [polynomial](../../../../../polynomial-split.md) $g$. Containment gives $X^N-1=gh$ for some [polynomial](../../../../../polynomial-split.md) $h$. Thus the [generator polynomial of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md) satisfies

$$
\boxed{g\mid X^N-1,\qquad C=(g)\text{ modulo }X^N-1.}
$$

For a nonzero code $g$ is also its monic word [polynomial](../../../../../polynomial-split.md) of smallest degree. For the zero code use $g=X^N-1$, whose residue is zero. Conversely every monic divisor defines a [cyclic code](../../../../../cyclic-code.md), proving the full correspondence.

Over $\mathbb F_2$,

$$
X^5-1=(X+1)(X^4+X^3+X^2+X+1).
$$

The quartic factor has no root in $\mathbb F_2$. The only monic irreducible quadratic over this field is $X^2+X+1$, and division leaves remainder $X+1$, so the quartic is not divisible by it. A reducible quartic with no linear factor would have two irreducible quadratic factors; hence this quartic is irreducible. There are exactly four [binary cyclic codes of length five](../../../../../binary-cyclic-codes-of-length-five.md), given by the [generator polynomials of a cyclic code](../../../../../generator-polynomial-of-a-cyclic-code.md)

$$
\boxed{1,\quad X+1,\quad X^4+X^3+X^2+X+1,\quad X^5-1.}
$$

They are respectively the full space, the even-weight code, the repetition code and the zero code, with dimensions $5,4,1,0$.

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

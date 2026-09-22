<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The nonzero [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) forces $b\ne0$. At $P$, the derivative with respect to $y$ is $b$ and that with respect to $x$ is zero, so the tangent is $y=0$. Substitution gives $x^2(x+b)=0$: its third point is $(-b,0)$. Applying the negation formula gives

$$
\boxed{-2P=(-b,0),\qquad2P=(-b,b(a-1)).}
$$

The line through $P$ and $2P$ has slope $1-a$, because their x-coordinates are distinct. Substitution of $y=(1-a)x$ gives

$$
x\bigl(x+b\bigr)\bigl(x+a-1\bigr)=0.
$$

Its third point is $(1-a,(1-a)^2)$, interpreted with multiplicity if it coincides with a previously used point. Negating it yields

$$
\boxed{-3P=(1-a,(1-a)^2),\qquad3P=(1-a,a-b-1).}
$$

By associativity, $5P=O$ exactly when $3P=-2P$. Equality of their x-coordinates forces $1-a=-b$, and when $a=b+1$ their y-coordinates also agree and are zero. Therefore

$$
\boxed{5P=O\iff a=b+1.}
$$

Since $P\ne O$, its order in this case is exactly five. These are the [torsion multiples in a two-parameter Weierstrass family](../../../../../../torsion-multiples-in-a-two-parameter-weierstrass-family.md) formulas.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

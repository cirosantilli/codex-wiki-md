<h1 id="13g/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the nonconstant bijective map as $p/q$ with coprime [polynomials](../../../../../../polynomial-split.md) and set $d=\max(\deg p,\deg q)$. For a finite value $w$, its finite preimages solve $p(z)-wq(z)=0$. Except for a possible leading-coefficient cancellation value, this [polynomial](../../../../../../polynomial-split.md) has degree $d$.

Multiple roots can occur only at zeros of $p'q-pq'$, since at a root $q\ne0$ by coprimality. This [derivative](../../../../../../derivative.md) numerator is a nonzero [polynomial](../../../../../../polynomial-split.md) for a nonconstant rational map. There are therefore only finitely many finite critical values to exclude. Choose $w$ outside them and outside the leading cancellation value. The [fundamental theorem of algebra](../../../../../../fundamental-theorem-of-algebra.md) then gives exactly $d$ distinct finite preimages. Bijectivity forces $d=1$.

Hence

$$
\boxed{f(z)=\frac{az+b}{cz+d_0},\qquad ad_0-bc\ne0,}
$$

which is a [Möbius transformation](../../../../../../mobius-transformation.md). Conversely, the inverse is $(d_0w-b)/(a-cw)$, interpreted at its [pole](../../../../../../pole.md) and at infinity, proving bijectivity on the [Riemann sphere](../../../../../../riemann-sphere.md). The argument also establishes the generic-preimage interpretation of the [degree of a rational map of the Riemann sphere](../../../../../../degree-of-a-rational-map-of-the-riemann-sphere.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [13G](../../13g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

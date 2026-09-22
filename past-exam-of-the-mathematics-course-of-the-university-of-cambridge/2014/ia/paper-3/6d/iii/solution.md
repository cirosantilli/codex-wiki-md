<h1 id="6d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write a [matrix](../../../../../../matrix.md) in the [upper unitriangular group](../../../../../../upper-unitriangular-group.md) as $M=I+A$. Here $A^3=0$, and its only potentially nonzero entry in $A^2$ is $(A^2)_{13}=ab$. The [binomial theorem](../../../../../../binomial-theorem.md) therefore gives the [unitriangular matrix power formula](../../../../../../unitriangular-matrix-power-formula.md)

$$
M^j=I+jA+\binom j2 A^2.
$$

For an odd [prime number](../../../../../../prime-number.md) $p$, both $p$ and $\binom p2=p(p-1)/2$ vanish in the [finite field](../../../../../../finite-field.md) $\mathbb F_p$. Thus $M^p=I$. A nonidentity $M$ has order dividing the prime $p$ (by the same exponent-division argument as in part (i)), and so has order exactly $p$.

For $p=2$, take $a=b=1$ and $x=0$. Then $M^2=I+A^2\ne I$, while $M^4=(I+A^2)^2=I$. This element has order $4$, not $2$. Hence **every nonidentity element has order $p$ exactly for odd $p$**. The counterexample at $p=2$ accounts for the quadratic term in the [matrix](../../../../../../matrix.md) power formula.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

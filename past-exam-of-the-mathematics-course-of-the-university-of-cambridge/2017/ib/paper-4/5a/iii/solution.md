<h1 id="5a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Evaluate $R_n$ at $x=1$ using $(x^2-1)^n=(x-1)^n(x+1)^n$. In the [Leibniz rule](../../../../../../leibniz-rule.md) for the $n$th [derivative](../../../../../../derivative.md), every term vanishes at $1$ except the term putting all $n$ [derivatives](../../../../../../derivative.md) on $(x-1)^n$. Therefore $R_n(1)=n!2^n$. Combining this with $P_n(1)=1$ gives the normalisation in the [Rodrigues' formula](../../../../../../rodrigues-formula.md):

$$
\boxed{\alpha_n=\frac1{2^n n!},\qquad P_n(x)=\frac1{2^n n!}\frac{d^n}{dx^n}(x^2-1)^n}.
$$

For $n=0$, the formula gives $\alpha_0=1$, as required. As an independent check, the leading term of $R_n$ is $(2n)!x^n/n!$, so the resulting [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md) of $P_n$ is $(2n)!/(2^n(n!)^2)$, consistent with the [Legendre polynomial recurrence relation](../../../../../../legendre-polynomial-recurrence-relation.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5A](../../5a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

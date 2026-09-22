<h1 id="7d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $x^2\equiv-1\pmod p$. Then $x\ne0$ modulo the [prime number](../../../../../../prime-number.md) $p$, so [Fermat's little theorem](../../../../../../fermat-little-theorem.md) gives $x^{p-1}\equiv1\pmod p$. But $p=4m+3$ makes $(p-1)/2=2m+1$ odd, and therefore

$$
x^{p-1}=(x^2)^{(p-1)/2}\equiv(-1)^{2m+1}=-1\pmod p.
$$

This contradicts $1\not\equiv-1\pmod p$, since $p$ is odd. Thus **$-1$ is not a [quadratic residue](../../../../../../quadratic-residue.md) modulo $p$**. Apply part (a) to the [finite field](../../../../../../finite-field.md) $F=\mathbb F_p$: the pairs $F^2$ with the given operations form a [field](../../../../../../field.md), and there are $p$ choices for each coordinate, so its [cardinality](../../../../../../cardinality.md) is $\boxed{p^2}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7D](../../7d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

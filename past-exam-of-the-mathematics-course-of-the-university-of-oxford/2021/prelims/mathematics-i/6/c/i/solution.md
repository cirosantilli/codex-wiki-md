<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

If the [prime number](../../../../../../../prime-number-split.md) $p$ divides $2^q-1$, then $p\ne2$, because $2^q-1$ is odd. Thus the residue of $2$ is an element of the [multiplicative group of a finite field](../../../../../../../multiplicative-group-of-a-finite-field.md) $\mathbb Z_p$, and $2^q\equiv1\pmod p$.

Let $d$ be its [order of a group element](../../../../../../../order-of-a-group-element.md). The [integer division](../../../../../../../integer-division.md) writes $q=ad+r$ with $0\leq r<d$. Then $1\equiv2^q\equiv(2^d)^a2^r\equiv2^r\pmod p$, so minimality of $d$ gives $r=0$. Hence $d$ divides $q$. Since $q$ is a [prime number](../../../../../../../prime-number-split.md), $d=1$ or $d=q$. The former would give $2\equiv1\pmod p$, which would mean $p$ divides $1$, an impossibility. Consequently

$$
\boxed{\operatorname{ord}_p(2)=q.}
$$

## ↑ Ancestors (13)

1. [i](../i.md)
2. [c](../../c.md)
3. [6](../../../6.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

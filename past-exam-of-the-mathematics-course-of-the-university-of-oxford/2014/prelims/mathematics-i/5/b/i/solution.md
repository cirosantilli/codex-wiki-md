<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $n=o(g)$. A [group homomorphism](../../../../../../../group-homomorphism.md) preserves powers and the [identity element](../../../../../../../identity-element.md), so

$$
\phi(g)^n=\phi(g^n)=\phi(e)=e_H.
$$

The preceding divisibility property gives

$$
\boxed{o(\phi(g))\mid o(g).}
$$

Now assume $\phi$ is surjective and choose $h\in H$ of order $m$. Take a preimage $g$ of $h$, and write $o(g)=mr$, as the divisibility result permits. The element $g^r$ has order exactly $m$: its $m$th power is $e$, while $(g^r)^s=e$ implies $mr\mid rs$, hence $m\mid s$. Therefore **$G$ contains an element of order $m$**, namely $g^r$.

The preimage $g$ itself need not have order $m$; taking the suitable power is the essential step. The constructed element need not map to the original $h$. This proves that [element orders in a finite quotient occur in the original group](../../../../../../../element-orders-in-a-finite-quotient-occur-in-the-original-group.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

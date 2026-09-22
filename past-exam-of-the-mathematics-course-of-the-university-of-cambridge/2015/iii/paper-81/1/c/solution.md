<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Holstein–Primakoff transformation](../../../../../../holstein-primakoff-transformation.md) on the physical [occupation number](../../../../../../occupation-number.md) subspace $0\le n\le2S$. With the [canonical commutation relation](../../../../../../canonical-commutation-relation.md) $[a,a^\dagger]=1$, the ordered square root gives

$$
S^+|n\rangle=\sqrt{n(2S-n+1)}\,|n-1\rangle,\qquad S^-|n\rangle=\sqrt{(n+1)(2S-n)}\,|n+1\rangle.
$$

Both endpoints are respected: $S^+|0\rangle=0$ and $S^-|2S\rangle=0$. Consequently,

$$
[S^+,S^-]|n\rangle=\big[(n+1)(2S-n)-n(2S-n+1)\big]|n\rangle=2(S-n)|n\rangle=2S^z|n\rangle.
$$

Since these [Fock states](../../../../../../fock-state.md) form a [basis](../../../../../../basis.md) of the physical spin space, **$[S^+,S^-]=2S^z$** there. Similarly $[S^z,S^\pm]=\pm S^\pm$. The [Holstein–Primakoff occupation constraint](../../../../../../holstein-primakoff-occupation-constraint.md) is essential: unrestricted bosonic occupation would not represent a spin-$S$ [Hilbert space](../../../../../../hilbert-space-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $M=0$, take the empty filtration. Otherwise a nonzero quotient $Q=M/M_i$ is a finitely generated [module](../../../../../../module-mathematics.md). Because $R$ has the [ascending chain condition](../../../../../../ascending-chain-condition.md) on ideals, the nonempty collection of annihilators of nonzero elements of $Q$ has a maximal element. Part (b), applied to $Q$, supplies $q\ne0$ with a [prime ideal](../../../../../../prime-ideal.md) $P=\operatorname{Ann}(q)$.

The map $R\to Rq$, $r\mapsto rq$, is surjective with kernel $P$. The [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) gives $Rq\cong R/P$. Let $M_{i+1}$ be the inverse image of $Rq$ under $M\to Q$. Then

$$
M_i\subsetneq M_{i+1},\qquad \boxed{M_{i+1}/M_i\cong R/P.}
$$

Repeat whenever the quotient remains nonzero. An infinite repetition would give a strictly ascending chain of [submodules](../../../../../../submodule.md) of the [Noetherian module](../../../../../../noetherian-module.md) $M$, contradicting part (a). Thus the process stops after finitely many steps, necessarily at $M$.

**This constructs the required [prime filtration](../../../../../../prime-filtration.md)** $0=M_0\subsetneq\cdots\subsetneq M_l=M$, with each successive quotient $R/P_i$ for a prime $P_i$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

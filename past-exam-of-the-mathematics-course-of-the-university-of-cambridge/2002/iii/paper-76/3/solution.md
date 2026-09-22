<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $x_1,\ldots,x_s$ contain all [free variables](../../../../../free-variable.md) of $M$. The [lambda term](../../../../../lambda-term.md) $M$ is a [solvable lambda term](../../../../../solvable-lambda-term.md) if there are closed [lambda terms](../../../../../lambda-term.md) $P_1,\ldots,P_k$ such that

$$
(\lambda x_1\cdots x_s.M)P_1\cdots P_k\equiv_\beta I,\qquad I=\lambda x.x.
$$

Additional arguments beyond the first $s$ are allowed. A [head normal form](../../../../../head-normal-form.md) is a term $\lambda u_1\cdots u_n.yM_1\cdots M_r$ with a variable at the head; its arguments need not be beta-normal.

If $M$ reduces to this [head normal form](../../../../../head-normal-form.md), close its [free variables](../../../../../free-variable.md) and supply every resulting initial binder with the same closed projection

$$
P=\lambda a_1\cdots a_r.I
$$

(take $P=I$ when $r=0$). The head variable becomes $P$ and discards all $r$ argument terms, even divergent ones, leaving $I$. Thus a [head normal form](../../../../../head-normal-form.md) implies solvability.

Conversely suppose a closure and applications of $M$ yield $I$. The [standardization theorem for beta reduction](../../../../../standardization-theorem-for-beta-reduction.md) supplies a finite successful head-reduction sequence. Until $M$ exposes a head variable, its head contractions lie within $M$: a closing substitution cannot create a new head redex there, and supplied arguments cannot be used until an initial abstraction is exposed. Each such contraction commutes with the closing [capture-avoiding substitution](../../../../../capture-avoiding-substitution.md). Project the successful head computation back onto $M$, ignoring contractions in supplied arguments and the consumption of its initial binders. If this projected head computation did not reach a variable-headed spine, the full computation could not reach $I$ either. It therefore gives a finite head reduction of $M$ to a [head normal form](../../../../../head-normal-form.md). Consequently

$$
\boxed{M\text{ is solvable}\iff M\text{ has a head normal form}.}
$$

The same head-trace argument shows that an [unsolvable lambda term](../../../../../unsolvable-lambda-term.md) stays unsolvable under substitution and application. This also justifies the unsolvability conclusion in the preceding solution.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

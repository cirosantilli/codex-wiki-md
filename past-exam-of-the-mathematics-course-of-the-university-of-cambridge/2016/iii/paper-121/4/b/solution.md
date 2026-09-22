<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One can take $\boxed{\alpha=\omega+1}$. Finite induction gives $L_n=V_n$ for every finite $n$: every subset of a finite level is definable using its finitely many elements as parameters. Hence $L_\omega=V_\omega$, the set of [hereditarily finite sets](../../../../../../hereditarily-finite-set.md).

Now reason inside the [constructible universe](../../../../../../constructible-universe.md) $L$, a model of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md). The set $L_\omega$ is countable there, and there are countably many [first-order formulas](../../../../../../first-order-formula.md) and finite parameter tuples. Thus $L_{\omega+1}=\operatorname{Def}(L_\omega)$ is countable in $L$. But the [constructible power set](../../../../../../constructible-power-set.md) $\mathcal P^L(\omega)$ is uncountable in $L$ by the [Cantor theorem](../../../../../../cantor-s-theorem.md). Choose

$$
r\in\mathcal P^L(\omega)\setminus L_{\omega+1}.
$$

This $r$ is constructible and a subset of $\omega$, so $r\subseteq V_\omega$ and $r\in V_{\omega+1}$. Therefore

$$
\boxed{r\in L\cap V_{\omega+1}\setminus L_{\omega+1}}.
$$

All comparisons were made inside $L$; this avoids assuming that the constructible reals are uncountable in the ambient universe. The witness remains valid externally because the two structures use the same $r$, the same $V_\omega$, and the same constructible level. Thus [constructible sets of low rank can appear at later stages](../../../../../../constructible-sets-of-low-rank-can-appear-at-later-stages.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

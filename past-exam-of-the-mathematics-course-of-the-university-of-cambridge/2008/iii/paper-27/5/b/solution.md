<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [constructible hierarchy](../../../../../../constructible-hierarchy.md) is $L_0=\varnothing$, $L_{\alpha+1}=\operatorname{Def}(L_\alpha)$ and $L_\lambda=\bigcup_{\alpha<\lambda}L_\alpha$ at limits; $L=\bigcup_{\alpha\in\mathrm{Ord}}L_\alpha$. Definability allows parameters from the current level. Satisfaction for a set-sized level is recursively definable, so this is a definable class construction in [ZF](../../../../../../zermelo-fraenkel-set-theory.md). Induction shows its levels are [sets](../../../../../../set-split.md), increasing and transitive, and contain every ordinal below their height.

We give the necessary reflection argument to check its full axiom schemes. For any finite collection $\Sigma$ of formulas, close it under subformulas and negation. Starting at any level containing the desired parameters, for every existential subformula and parameter tuple in that level for which a witness in $L$ exists, take the least constructibility stage containing such a witness. These least stages are uniquely definable ordinals; ambient replacement bounds all of them. Enlarge to a level beyond the bound, repeat countably many times, and take the union stage $\beta$. Every existential witness required by a tuple in $L_\beta$ is then already in $L_\beta$, because the tuple appeared at a previous stage. Induction on the finitely many formulas gives

$$
L_\beta\models\varphi(\bar a)\quad\Longleftrightarrow\quad L\models\varphi(\bar a)
\qquad(\varphi\in\Sigma,\ \bar a\in L_\beta).
$$

This uses a truth definition for each fixed finite list, not a truth predicate for the entire ambient universe.

Extensionality and foundation hold in $L$ by transitivity. Pairs and unions of elements of a level are definable subsets of a sufficiently large transitive level. The hereditarily finite [sets](../../../../../../set-split.md) appear in $L_\omega$, and the [set](../../../../../../set-split.md) of its finite ordinals is definable there, so $\omega\in L$ and infinity holds. For separation on $a\in L$ with parameters in $L$, reflect the relevant formula into a level $L_\beta$ containing them and $a$. The desired subset of $a$ is then definable over $L_\beta$, so belongs to $L_{\beta+1}$.

For replacement, suppose $L$ says $\varphi$ defines a unique value in $L$ for each $x\in a$. The relativization $\varphi^L$ is an ambient formula. Ambient replacement collects its values, and replacement applied to their least constructibility stages bounds them all in some $L_\gamma$. Reflect the formula in a still larger level containing $a$, the parameters and those values. The range is now a definable subset of that level, so lies in $L$. For power [set](../../../../../../set-split.md), the ambient [set](../../../../../../set-split.md) $\mathcal P(a)\cap L$ exists by separation. Its members' constructibility stages are bounded, say all members lie in $L_\gamma$ with $a\in L_\gamma$. Then

$$
\mathcal P(a)\cap L=\{b\in L_\gamma:b\subseteq a\}
$$

is definable over $L_\gamma$; transitivity makes the displayed bounded subset condition absolute. Thus this internal power [set](../../../../../../set-split.md) also belongs to $L$. We have proved $L\models\mathsf{ZF}$.

Finally define its canonical well-order recursively. At a successor stage, code a definition by its formula number and its finite tuple of parameters, ordered by the already constructed well-order of the previous level. Order new elements by their least definition codes, preserving earlier elements first. At a limit take the coherent union, with first-appearance stages providing the primary comparison. Induction makes every level well-ordered and gives a definable class well-order of $L$. Its restriction to any [set](../../../../../../set-split.md) in $L$ belongs to $L$ by separation, so every such [set](../../../../../../set-split.md) is internally well-orderable. Hence

$$
\boxed{L\models\mathsf{ZFC},\qquad\operatorname{Con}(\mathsf{ZF})\Rightarrow\operatorname{Con}(\mathsf{ZFC}).}
$$

The implication is a relative consistency argument, not a proof by [ZF](../../../../../../zermelo-fraenkel-set-theory.md) of its own consistency.

Now [Shepherdson's wall](../../../../../../shepherdson-s-wall.md) explains the limitation of this method. If $W$ is a transitive inner model containing all ordinals, its constructible levels agree with the ambient ones. At successors both compute definable subsets of the same set-sized structure, with the same finite formulas and parameters; at limits both take the same union. Thus $L^W=L\subseteq W$. In an ambient universe satisfying $V=L$, this forces $W=V$. Therefore a uniform inner-model construction valid in every model of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) cannot always yield an inner model with $V\ne L$, nor one failing choice or CH: apply the proposed construction in a model of [ZF](../../../../../../zermelo-fraenkel-set-theory.md) with $V=L$. The construction of $L$ removes nonconstructible [sets](../../../../../../set-split.md) and proves positive choice consistency; it cannot manufacture the nonconstructible [sets](../../../../../../set-split.md) needed for those negative results.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $K_s$ be the finite approximation to the [halting problem](../../../../../halting-problem.md) obtained by running the first $s$ programs for $s$ steps, so $K_s\subseteq K_{s+1}$ and $K=\bigcup_sK_s$ is not [computable](../../../../../computable-set.md). For $x<y<z$, define the [recursive triple colouring with no computable infinite homogeneous set](../../../../../recursive-triple-colouring-with-no-computable-infinite-homogeneous-set.md) by

$$
c(\{x,y,z\})=\begin{cases}0&K_y\cap[0,x]=K_z\cap[0,x],\\1&\text{otherwise}.\end{cases}
$$

This is a [total computable function](../../../../../total-computable-function.md). Here homogeneous sets are required to be infinite: finite homogeneous sets certainly exist. An infinite homogeneous $H$ cannot have colour one. Fix $x\in H$; the finite approximation below $x$ eventually stabilizes, so two sufficiently large $y<z$ in $H$ give colour zero. If $H$ has colour zero, choose $x<y$ in $H$ with $x\ge e$. For arbitrarily large $z\in H$, homogeneity gives $K_y\cap[0,x]=K_z\cap[0,x]$, and hence $K_y\cap[0,x]=K\cap[0,x]$. Thus $H$ computes membership of $e$ in $K$. A [computable](../../../../../computable-set.md) infinite $H$ would make the [halting problem](../../../../../halting-problem.md) computable, a contradiction.

For the uncountable [partition relation](../../../../../partition-relation.md), the [Erdős-Rado theorem for finite arities](../../../../../erdos-rado-theorem-for-finite-arities.md) states that for every infinite [cardinal](../../../../../cardinal-number.md) $\kappa$ and integer $n\ge1$,

$$
\boxed{\beth_{n-1}(\kappa)^+\longrightarrow(\kappa^+)^n_\kappa},\qquad
\beth_0(\kappa)=\kappa,\quad\beth_{r+1}(\kappa)=2^{\beth_r(\kappa)}.
$$

The case $n=1$ is the [pigeonhole principle](../../../../../pigeonhole-principle.md): a union of $\kappa$ sets of size at most $\kappa$ cannot have size $\kappa^+$. Suppose the assertion holds for $n-1$. Put $\mu=\beth_{n-2}(\kappa)$ and $\lambda=(2^\mu)^+$, and let $c:[\lambda]^n\to\kappa$. We give the [closed elementary-submodel construction of an end-homogeneous sequence](../../../../../closed-elementary-submodel-construction-of-an-end-homogeneous-sequence.md), which avoids intersecting a decreasing family of reservoirs at a limit stage.

Take a sufficiently large regular $\chi$ and an [elementary substructure](../../../../../elementary-substructure.md) $M\prec H_\chi$ with $|M|=2^\mu$, containing $c,\lambda$ and all ordinals below $\mu^+$, and closed under sequences of length at most $\mu$. Such an $M$ is obtained by $\mu^+$ successive [Skolem hull](../../../../../skolem-hull.md) closures: $(2^\mu)^\mu=2^\mu$, and the regularity of $\mu^+$ puts any at-most-$\mu$-long sequence from the union inside one stage. Put $\beta=\sup(M\cap\lambda)<\lambda$. The set $M\cap\lambda$ has no greatest element, since taking an ordinal successor is definable in $M$, so $\beta\notin M$.

Recursively choose an increasing sequence $\langle x_\xi:\xi<\mu^+\rangle$ in $M\cap\lambda$. At stage $\xi$, its earlier set $A$ has size at most $\mu$, and the colour table $g(u)=c(u\cup\{\beta\})$ on $[A]^{n-1}$ has size at most $\mu$. Both $A$ and this table belong to $M$ by its closure. The set

$$
X=\{t<\lambda:t>\sup A\text{ and }(\forall u\in[A]^{n-1})\ c(u\cup\{t\})=g(u)\}
$$

belongs to $M$ and is nonempty because it contains $\beta$. [Elementarity](../../../../../elementarity.md) supplies $x_\xi\in X\cap M$. Consequently the colour of each $n$-tuple from the resulting sequence depends only on its first $n-1$ entries. The [induction hypothesis](../../../../../induction-hypothesis.md) applied to these entries gives a homogeneous subsequence of size $\kappa^+$, proving the result.

Infinite exponents behave differently with the [axiom of choice](../../../../../axiom-of-choice.md). On the countably infinite subsets of any infinite [cardinal](../../../../../cardinal-number.md) $\lambda$, choose a representative of each equivalence class modulo [finite symmetric difference](../../../../../finite-symmetric-difference.md). Colour a set $A$ by the parity of $|A\mathbin\triangle R_A|$. Removing one point flips its colour. Every infinite proposed homogeneous set contains an increasing sequence of order type $\omega$, and that sequence and its tail have opposite colours. Thus the [finite-symmetric-difference colouring of infinite subsets](../../../../../finite-symmetric-difference-colouring-of-infinite-subsets.md) gives $\lambda\not\longrightarrow(\omega)^\omega_2$, whether the domain consists of all countably infinite subsets or only those of order type $\omega$. There is no unrestricted infinite-arity counterpart to the displayed finite-arity theorem in [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

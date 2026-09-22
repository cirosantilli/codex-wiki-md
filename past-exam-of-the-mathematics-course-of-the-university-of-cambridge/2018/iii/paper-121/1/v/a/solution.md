<h1 id="1/v/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We construct the two [transitive models](../../../../../../../transitive-model.md) together, taking care that the later collapse really retains the earlier model. First, a [worldly cardinal](../../../../../../../worldly-cardinal.md) $\kappa$ is greater than $\omega_1$: [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md) in $V_\kappa$ contains the full [power set](../../../../../../../power-set.md) $\mathcal P(\omega)$, and the [axiom of choice](../../../../../../../axiom-of-choice.md) there gives a [bijection](../../../../../../../bijection.md) between it and an ordinal $\gamma<\kappa$. That power set is externally uncountable by [Cantor theorem](../../../../../../../cantor-s-theorem.md), so $\gamma\geq\omega_1$. Infinity rules out the finite cardinals and $\omega$ before this argument is applied.

By the [Downward Lowenheim-Skolem theorem](../../../../../../../downward-lowenheim-skolem-theorem.md), choose a countable [elementary substructure](../../../../../../../elementary-substructure.md) $X\prec(V_\kappa,\in)$. Its inherited membership is a [well-founded relation](../../../../../../../well-founded-relation.md), and elementarity transfers extensionality from $V_\kappa$. Apply the [Mostowski collapse theorem](../../../../../../../mostowski-collapse-theorem.md) to obtain a [countable transitive model](../../../../../../../countable-transitive-model.md) $M$ of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md). Because $M$ is a countable [transitive set](../../../../../../../transitive-set.md), it is a [hereditarily countable set](../../../../../../../hereditarily-countable-set.md) and its [rank of a set](../../../../../../../rank-of-a-set.md) is below $\omega_1$. In particular, $M\in V_\kappa$.

Now take the [Skolem hull](../../../../../../../skolem-hull.md) in $V_\kappa$ of the seed

$$
S=\omega_1\cup M\cup\{\omega_1,M\}.
$$

Call it $H$. The seed has external cardinality $\aleph_1$ and lies inside $V_\kappa$. The hull is an [elementary substructure](../../../../../../../elementary-substructure.md) of $V_\kappa$ with $|H|=\aleph_1$: closure under countably many finitary Skolem functions gives the upper bound, and $\omega_1\subseteq H$ gives the lower bound. Let $\pi:H\to N$ be its [Mostowski collapse theorem](../../../../../../../mostowski-collapse-theorem.md) map. Then $N$ is a [transitive model](../../../../../../../transitive-model.md) of [ZFC](../../../../../../../zermelo-fraenkel-set-theory-with-choice.md).

The [transitive collapse fixes transitive subsets](../../../../../../../transitive-collapse-fixes-transitive-subsets.md) lemma gives $\pi(m)=m$ for every $m\in M$, since $M\subseteq H$ is transitive. Since also $M\in H$, the collapse sends that element to $M$ itself. Thus $M\in N$, and transitivity of $N$ yields the required inclusion:

$$
\boxed{M\in N\quad\text{and hence}\quad M\subseteq N.}
$$

This is the construction of [nested transitive models from a worldly cardinal](../../../../../../../nested-transitive-models-from-a-worldly-cardinal.md); the next two parts verify its size and ordinal requirements.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [V](../../v.md)
3. [1](../../../1.md)
4. [Paper 121](../../../../paper-121-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Dense Bogolyubov-Ruzsa lemma](../../../../../../dense-bogolyubov-ruzsa-lemma.md) says that, for every $\alpha>0$, if $S$ has density at least $\alpha$ in a cyclic group of prime order, then $2S-2S$ contains a proper [generalized arithmetic progression](../../../../../../generalized-arithmetic-progression.md) of rank $O_\alpha(1)$ and size $\Omega_\alpha(|G|)$.

Now suppose $A\subseteq\mathbb Z$ and $|A+A|\leq K|A|$. The [Ruzsa modelling lemma](../../../../../../ruzsa-modelling-lemma.md), taken at a sufficiently high fixed Freiman order, supplies $A'\subseteq A$ with $|A'|\geq|A|/2$ and a Freiman isomorphism from $A'$ to a subset $S\subseteq\mathbb Z/q\mathbb Z$, where $q$ is prime, $q=O_K(|A|)$, and $|S|/q\gg_K1$. Apply the dense Bogolyubov-Ruzsa lemma to $S$ and transfer the resulting progression back through the Freiman model. We obtain a proper progression

$$
P_0\subseteq2A'-2A'\subseteq2A-2A
$$

of rank $O_K(1)$ and size $|P_0|\gg_K|A|$.

The [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md) gives

$$
|A+P_0|\leq|3A-2A|\leq K^5|A|.
$$

There are $|A||P_0|$ pairs $(a,p)$ with $a\in A$ and $p\in P_0$, distributed among the sums in $A+P_0$. Some $x$ therefore has at least $K^{-5}|P_0|\gg_K|A|$ representations $x=a+p$. Equivalently,

$$
|A\cap(x-P_0)|\gg_K|A|.
$$

Set $P=x-P_0$. Translation and negation preserve properness and rank. Moreover $P_0\subseteq2A-2A$ and another use of Plünnecke gives $|P|\leq K^4|A|$. Thus

$$
|A\cap P|\gg_K|A|\gg_K|P|,
$$

as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

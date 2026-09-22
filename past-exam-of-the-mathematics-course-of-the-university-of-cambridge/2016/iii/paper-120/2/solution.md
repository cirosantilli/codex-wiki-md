<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a finite position $s\in A^{<\omega}$, let $[s]$ be the [cylinder set](../../../../../cylinder-set.md) of infinite plays extending $s$. Because the factors have the [discrete topology](../../../../../discrete-space.md), these [cylinder sets](../../../../../cylinder-set.md) form a basis for the [product topology](../../../../../product-topology.md). Put

$$
D=\{s:[s]\subseteq G\}.
$$

Membership in $D$ means that I has already secured the outcome, regardless of future moves. Since $G$ is an [open set](../../../../../open-set.md), a play belongs to $G$ exactly when one of its prefixes belongs to $D$.

Build the [winning-position attractor in an infinite game](../../../../../winning-position-attractor-in-an-infinite-game.md) by [transfinite recursion](../../../../../transfinite-recursion.md). Start with $W_0=D$, use unions at limit [ordinals](../../../../../ordinal.md), and set

$$
W_{\alpha+1}=D
\cup\{s:|s|\text{ is even and }\exists a\in A\ (sa\in W_\alpha)\}
\cup\{s:|s|\text{ is odd and }\forall a\in A\ (sa\in W_\alpha)\}.
$$

This sequence is increasing: the defining operation is [order-preserving](../../../../../order-preserving-function.md), and $W_0\subseteq W_1$. It stabilizes at some ordinal. Indeed, if it strictly increased at every successor stage below the successor [cardinal number](../../../../../cardinal-number.md) of $|A^{<\omega}|$, choosing one newly added position per stage would inject that larger cardinal into $A^{<\omega}$. Denote the stable set by $W$. This constructs the needed [fixed point](../../../../../fixed-point.md) directly, without an appeal to an unstated [fixed-point theorem](../../../../../fixed-point-theorem.md).

Every position in $W$ has a least entry [ordinal](../../../../../ordinal.md), its rank. Rank zero means membership in $D$. A positive rank is a successor $\alpha+1$: at an I-position some extension belongs to $W_\alpha$, while at a II-position every extension does. If the [empty word](../../../../../empty-word.md) belongs to $W$, I always chooses an extension of smaller rank until $D$ is reached. II's choices also decrease rank before that happens. There is no infinite strictly decreasing sequence of [ordinals](../../../../../ordinal.md), so some finite prefix lies in $D$. This is a [winning strategy in an infinite game](../../../../../winning-strategy-in-an-infinite-game.md) for I.

If the [empty word](../../../../../empty-word.md) is outside $W$, the [fixed point](../../../../../fixed-point.md) equation says that every extension of an I-position outside $W$ is still outside $W$, and that a II-position outside $W$ has at least one extension outside $W$. II chooses such an extension. Every resulting prefix avoids $D$, hence the whole play avoids $G$ by openness. This is a [winning strategy in an infinite game](../../../../../winning-strategy-in-an-infinite-game.md) for II.

The choices can be made simultaneously by fixing a [well-order](../../../../../well-order.md) of $A$, as allowed by the usual [axiom of choice](../../../../../axiom-of-choice.md). The argument does not assume that $A$ is countable. **Every such open game is determined**:

$$
\boxed{\varepsilon\in W\Rightarrow\text{I wins};\qquad
\varepsilon\notin W\Rightarrow\text{II wins}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 120](../../paper-120-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

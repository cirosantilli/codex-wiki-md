<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Commutative Gelfand--Naimark theorem](../../../../../../commutative-gelfand-naimark-theorem.md) states that a complex commutative unital [C-star algebra](../../../../../../c-star-algebra.md) $A$ is isometrically star-isomorphic to $C(\Phi_A)$ through its [Gelfand transform](../../../../../../gelfand-representation.md), with $\Phi_A$ a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md). The [l-infinity sequence space](../../../../../../l-infinity-sequence-space.md) is such an algebra under coordinatewise multiplication and conjugation, with the [supremum norm](../../../../../../supremum-norm.md). Therefore

$$
\boxed{K=\Phi_{\ell^\infty},\qquad \Gamma:\ell^\infty\longrightarrow C(K),\quad \Gamma(a)(\chi)=\chi(a)}
$$

gives the required isometric isomorphism.

Uniqueness as a [Banach space](../../../../../../banach-space-split.md) representation uses the [Banach–Stone theorem](../../../../../../banach-stone-theorem.md), rather than just uniqueness as an algebra representation. To justify the relevant theorem, the [Riesz-Markov-Kakutani representation theorem](../../../../../../riesz-markov-kakutani-representation-theorem.md) gives

$$
\operatorname{ext}B_{C(K)^*}=\{\alpha\delta_t:t\in K,\ |\alpha|=1\},
$$

the [extreme points of the dual unit ball of C(K)](../../../../../../extreme-points-of-the-dual-unit-ball-of-c-k.md). A norm-one measure whose [variation measure](../../../../../../variation-measure.md) is not concentrated at one point splits into two normalized restrictions to disjoint sets of positive variation, and so is not extreme. Conversely, equality in the variation bound shows that any decomposition of $\alpha\delta_t$ into the average of two dual-unit-ball elements forces both to be $\alpha\delta_t$: after removing the phase, the two measures must be positive and their average is concentrated at $t$.

If $U:C(K)\to C(L)$ is a surjective linear [isometry](../../../../../../isometry.md), its [dual map](../../../../../../transpose-of-a-linear-map.md) preserves these [extreme points](../../../../../../extreme-point.md) and their scalar orbits. Hence $U^*\delta_s=u(s)\delta_{h(s)}$ for a bijection $h:L\to K$ and $|u(s)|=1$. Evaluating at $1$ gives the continuous function $u=U1$, while

$$
f(h(s))=\frac{(Uf)(s)}{u(s)}\quad(f\in C(K))
$$

shows that $h$ is continuous, since continuous functions determine the topology of a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md). It is consequently a [homeomorphism](../../../../../../homeomorphism.md). Thus any other compact space representing $\ell^\infty$ is homeomorphic to this $K$. The [Banach–Stone theorem](../../../../../../banach-stone-theorem.md) is also stated in [Leonard Tomczak's notes on András Zsák's functional analysis lectures](https://math.berkeley.edu/~ltomczak/notes/Lent2023/FuncAna_Notes.pdf).

Embed $\mathbb N$ by the [evaluation characters](../../../../../../evaluation-character.md) $\iota(n)(a)=a_n$. They are distinct because the coordinate [indicator functions](../../../../../../indicator-function.md) $e_n$ distinguish them. Moreover, $e_n^2=e_n$, so every character has $\chi(e_n)\in\{0,1\}$. If $\chi(e_n)=1$, then

$$
\chi(a)=\chi(ae_n)=a_n\chi(e_n)=a_n,
$$

and hence $\chi=\iota(n)$. It follows that $\{\iota(n)\}=\{\chi:|\chi(e_n)-1|<1/2\}$ is open in $K$. Thus $\iota$ is a [homeomorphism](../../../../../../homeomorphism.md) from the discrete natural numbers onto its image.

To prove density, suppose $D=\overline{\iota(\mathbb N)}\ne K$. The [Urysohn lemma](../../../../../../urysohn-s-lemma.md) provides a nonzero $v\in C(K)$ vanishing on $D$. Write $v=\Gamma(a)$. Then $a_n=v(\iota(n))=0$ for all $n$, so $a=0$ and $v=0$, a contradiction. Every bounded function $b:\mathbb N\to\mathbb C$ is an element of $\ell^\infty$, and $\Gamma(b)$ is its continuous extension to $K$. Density makes this extension unique. Therefore

$$
\boxed{K\cong\beta\mathbb N,\qquad b\mapsto\Gamma(b)\text{ is the unique continuous extension of every bounded }b.}
$$

This identifies $K$ with the [Stone-Čech compactification of the natural numbers](../../../../../../stone-cech-compactification-of-the-natural-numbers.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

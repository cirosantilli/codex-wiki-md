<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $E_T,E_B,E_L,E_R$ be the [increasing events](../../../../../../../increasing-event.md) that an infinite simple open [ray in a graph](../../../../../../../ray-in-a-graph.md) starts at the indicated side and immediately leaves the box, with all later [graph vertices](../../../../../../../vertex-graph-theory.md) outside it. A corner exit is assigned according to the direction of its outgoing [edge](../../../../../../../edge-of-a-graph.md). The four events have the same [probability](../../../../../../../probability.md) $a_N$ by rotational symmetry. Their union is $D_N$ from the preceding step.

The [Harris-FKG inequality](../../../../../../../harris-fkg-inequality.md) applies to these exterior-ray events by approximation with finite connections to larger boxes and passage to decreasing limits. Positive association of the four [decreasing events](../../../../../../../decreasing-event.md) $E_s^c$, by iterating the [Harris-FKG inequality](../../../../../../../harris-fkg-inequality.md), gives

$$
1-\mathbb P(D_N)=\mathbb P\Bigl(\bigcap_s E_s^c\Bigr)
\ge\prod_s\mathbb P(E_s^c)=(1-a_N)^4.
$$

Equivalently, one may apply the preceding [square-root bound for increasing events](../../../../../../../square-root-bound-for-increasing-events.md) first to the two opposite-side unions and then to the two individual sides of one pair. Therefore

$$
a_N\ge1-(1-\mathbb P(D_N))^{1/4}\longrightarrow1.
$$

A [union bound](../../../../../../../boole-s-inequality.md) now shows

$$
\mathbb P(E_T\cap E_B)\ge1-2(1-a_N)
\ge1-2(1-\mathbb P(D_N))^{1/4}.
$$

Choose $N$ such that $1-\mathbb P(D_N)<(1/8)^4$. Then

$$
\boxed{\mathbb P(E_T\cap E_B)>3/4.}
$$

The infinite exterior clusters touched by these two sides need not be the same. The same argument works for dual boxes and any sufficiently large size; this permits the matching primal/dual contours used in the full proof.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 30](../../../../paper-30-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

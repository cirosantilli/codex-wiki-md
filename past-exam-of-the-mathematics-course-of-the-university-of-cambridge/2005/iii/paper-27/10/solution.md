<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Use the natural [partial order](../../../../../partially-ordered-set.md)

$$
x\le y\quad\Longleftrightarrow\quad x+y=y.
$$

The paper's shorthand $x\le x+y$ specifies the join order: more formally, $x\le z$ means $z=x+y$ for some $y$, which is equivalent to the displayed condition by [idempotence](../../../../../idempotence.md). Associativity, commutativity and idempotence make addition the [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) operation. Distributivity makes multiplication monotone, while absorption gives $xy\le x$ and $xy\le y$.

Let $g_1,\ldots,g_r$ generate the [incline](../../../../../incline.md). Distributivity writes every element as a nonempty finite join of monomials

$$
m(v)=g_1^{v_1}\cdots g_r^{v_r},\qquad v\in\mathbb N^r\setminus\{0\}.
$$

There is no assumed multiplicative identity: an exponent zero means omit that factor, and at least one factor remains. If $u\le v$ coordinatewise, absorption gives $m(v)\le m(u)$. If the two vectors are equal the conclusion is immediate; otherwise multiply $m(u)$ by the additional factors and apply absorption. For a polynomial with finite exponent support $A$, put $U_A=\{v:(\exists u\in A)\ u\le v\}$, its upward closure. If $U_A\supseteq U_B$, every monomial in $B$ is below some monomial in $A$, and consequently the join represented by $B$ is below the join represented by $A$.

We prove the [reverse-inclusion well-quasi-ordering of monomial ideals](../../../../../reverse-inclusion-well-quasi-ordering-of-monomial-ideals.md), often called [Maclagan's theorem](../../../../../reverse-inclusion-well-quasi-ordering-of-monomial-ideals.md), in the equivalent form that upward-closed subsets of $\mathbb N^r$ are well-quasi-ordered by reverse inclusion. Include the empty subset. For $r=1$, these are the tails $[n,\infty)$ and the empty set, corresponding to $\mathbb N\cup\{\infty\}$ in its usual well-order.

Induct on $r$. For an upward-closed $U\subseteq\mathbb N^r$, its slices $U_k=\{v\in\mathbb N^{r-1}:(v,k)\in U\}$ increase with $k$. Their union is upward closed and has finitely many minimal elements by the [Dickson lemma](../../../../../dickson-s-lemma.md); all those elements have appeared by some finite slice. Thus the slices eventually stabilize. Encode $U$ by the finite word of its pre-stabilization slices and its final stable slice. By the induction hypothesis, the slice order given by reverse inclusion is a [well-quasi-ordering](../../../../../well-quasi-ordering.md). The [Higman lemma](../../../../../higman-s-lemma.md) and [finite product closure of well-quasi-orderings](../../../../../finite-product-closure-of-well-quasi-orderings.md) make these word-and-tail encodings well-quasi-ordered.

For a good pair of encodings $U,V$, an increasing subsequence map $f$ satisfies $U_k\supseteq V_{f(k)}$ at every pre-stabilization position of $U$, and the final slice of $U$ contains the final slice of $V$. Since $f(k)\ge k$ and the $V$ slices increase, $U_k\supseteq V_k$ before stabilization. Afterwards the final-slice comparison also gives $U_k\supseteq V_k$. Hence $U\supseteq V$, proving the induction. The use of [Higman lemma](../../../../../higman-s-lemma.md) is essential: finite-subset reverse domination does not preserve an arbitrary well-quasi-order, as the [Rado order](../../../../../rado-order.md) shows.

Given any infinite sequence of incline elements, choose a finite monomial support $A_i$ for each. The result just proved gives $i<j$ with $U_{A_i}\supseteq U_{A_j}$, hence $x_i\ge x_j$. **Every finitely generated incline is therefore well-quasi-ordered by its reversed natural order.**

## ↑ Ancestors (10)

1. [10](../10.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

## ← Incoming links (2)

- [Solution](a/solution.md)
- [Solution](c/solution.md)

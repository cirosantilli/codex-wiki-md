<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For finite [rooted trees](../../../../../../rooted-tree.md) write $T\preceq S$ when there is an [injective function](../../../../../../injective-function.md) of vertices preserving [greatest common ancestors](../../../../../../lowest-common-ancestor.md), equivalently an infimum-preserving [rooted-tree homeomorphic embedding](../../../../../../homeomorphic-embedding-of-a-rooted-tree.md). No linear ordering of siblings is imposed. [Kruskal's tree theorem](../../../../../../kruskal-s-tree-theorem.md) says that every infinite [sequence](../../../../../../sequence.md) has an earlier tree embedding into a later tree: this embedding relation is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md).

The finite form uses a parameter $k$ to restrict the growth of the trees. It asserts the existence of a length $N=N(k)$ for which

$$
\boxed{|T_i|\leq k+i\ (1\leq i\leq N)\quad\Longrightarrow\quad(\exists i<j\leq N)\,T_i\preceq T_j.}
$$

Here $|T|$ is the number of vertices. The parameter $k$ is universally quantified; changing the starting index just shifts the parameter. This is [Friedman's finite form of Kruskal's theorem](../../../../../../friedman-s-finite-form-of-kruskal-s-theorem.md).

Fix $k$ and suppose there were arbitrarily long [sequences](../../../../../../sequence.md) violating the conclusion. Form a tree whose nodes are their finite prefixes, including the empty prefix. Choose one representative of each finite rooted-tree isomorphism type. At position $i$ there are only finitely many choices, since the tree has at most $k+i$ vertices. Hence this [finite bad-sequence tree](../../../../../../finite-bad-sequence-tree.md) is finitely branching. It has nodes at arbitrarily large heights by the supposed failure of the finite form. [König infinity lemma](../../../../../../konig-s-lemma.md) supplies an infinite branch. The branch is an infinite [sequence](../../../../../../sequence.md) $T_1,T_2,\ldots$ satisfying the size bounds and with no pair $i<j$ having $T_i\preceq T_j$, contradicting [Kruskal's tree theorem](../../../../../../kruskal-s-tree-theorem.md). Therefore the finite length exists for every $k$.

The significance is that this is a true statement about finite objects and [natural numbers](../../../../../../natural-number.md) which is not provable in [Peano arithmetic](../../../../../../peano-arithmetic.md); in fact it is not provable in the stronger [arithmetical transfinite recursion theory](../../../../../../arithmetical-transfinite-recursion-theory.md) in [second-order arithmetic](../../../../../../second-order-arithmetic.md), $\mathsf{ATR}_0$. It is a natural combinatorial instance of incompleteness. For fixed $k,N$, the condition can be checked by finite search over trees and injective vertex maps, so its uniform [arithmetic](../../../../../../arithmetic-split.md) form is $\forall k\,\exists N\,R(k,N)$ with a computable, indeed [primitive recursive](../../../../../../primitive-recursive-function.md), predicate $R$. Thus its least sufficient length is a [total computable function](../../../../../../total-computable-function.md), but its totality cannot be proved in those theories. Each fixed numerical instance can nevertheless be proved in [Peano arithmetic](../../../../../../peano-arithmetic.md) by verifying some particular finite witness. The obstruction concerns the uniform statement for all parameters, rather than the decidability of any one finite search.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

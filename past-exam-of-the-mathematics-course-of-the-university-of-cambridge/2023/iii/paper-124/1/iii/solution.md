<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We use the following consequence of the [Håstad switching lemma](../../../../../../hastad-switching-lemma.md). If an unbounded-fan-in layered AND/OR circuit has depth $d$ and size $S$, then after $d-1$ successive independent random restrictions, each retaining a suitably small proportion $p=\Theta(1/\log S)$ of the currently live variables, the restricted circuit is constant on the leaves of a decision tree of bounded depth with probability at least $3/4$. To prove this [switching-lemma depth reduction](../../../../../../switching-lemma-depth-reduction.md), first express the bottom layer as DNFs or CNFs, truncate any term wider than $O(\log S)$ because a random assignment satisfies or kills it except with probability $S^{-O(1)}$, and then apply the switching lemma with a union bound over at most $S$ gates. Replace each surviving bottom gate by its decision tree, switch DNF to CNF or conversely, and repeat. Choosing the constants so each round fails with probability at most $1/(4d)$ proves the claim by a union bound.

Suppose now that $S=\exp(o(n^{1/(d-1)}))$. After the $d-1$ rounds, the expected number of live variables is

$$
N=n\,p^{d-1}
=\frac{n}{O((\log S)^{d-1})}\longrightarrow\infty.
$$

A [Chernoff bound](../../../../../../chernoff-bound.md) shows that at least $N/2$ variables remain live with probability tending to one. Conditional on the set of live variables, the assigned variables contain, with probability bounded away from zero, sufficiently close to half zeros and half ones that the restricted majority function remains a nonconstant threshold function on $\Omega(N)$ live variables. By part (i), its [decision-tree depth](../../../../../../decision-tree-depth.md) is then $\Omega(N)$.

With positive probability both conclusions hold: the restricted circuit has bounded decision-tree depth, but the function it computes has depth tending to infinity. This contradiction proves

$$
\log S=\Omega(n^{1/(d-1)}),
\qquad
S\geq\exp\!\left(c_dn^{1/(d-1)}\right).
$$

For each fixed depth, the constants in the reduction may be chosen uniformly to give an absolute positive constant after the usual depth convention is fixed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

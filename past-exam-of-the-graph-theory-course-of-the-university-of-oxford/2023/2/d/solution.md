<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First reduce the [unicyclic graph](../../../../unicyclic-graph.md) to its unique [graph cycle](../../../../cycle-in-a-graph.md) $C$. Delete the [edges](../../../../edge-of-a-graph.md) of $C$ but retain every [vertex](../../../../vertex-graph-theory.md). The remaining [graph](../../../../graph-split.md) is a [forest](../../../../forest.md), since any surviving [graph cycle](../../../../cycle-in-a-graph.md) would be a second one in $G$. Each of its [connected components of a graph](../../../../component-graph-theory.md) contains a [vertex](../../../../vertex-graph-theory.md) of $C$: follow a [graph path](../../../../path-in-a-graph.md) to $C$ in the original [connected graph](../../../../connected-graph.md), stopping at the first [vertex](../../../../vertex-graph-theory.md) of $C$; this initial segment uses no [edge](../../../../edge-of-a-graph.md) of $C$.

No such [connected component of a graph](../../../../component-graph-theory.md) contains two [vertices](../../../../vertex-graph-theory.md) of $C$. Otherwise, on the [tree](../../../../tree-graph-theory-split.md) [graph path](../../../../path-in-a-graph.md) between them, choose two successive visits to $C$. The segment between these visits has no internal [vertex](../../../../vertex-graph-theory.md) on $C$ and uses no [edge](../../../../edge-of-a-graph.md) of $C$. Combining it with either connecting arc of $C$ gives a second [graph cycle](../../../../cycle-in-a-graph.md), a contradiction. Thus the remaining [graph](../../../../graph-split.md) consists of [trees](../../../../tree-graph-theory-split.md), each rooted at exactly one [vertex](../../../../vertex-graph-theory.md) of $C$.

After choosing a [proper vertex colouring](../../../../proper-vertex-coloring.md) of $C$ from $q$ colours, colour these [rooted trees](../../../../rooted-tree.md) away from their roots. Each of the $n-\ell$ off-[graph cycle](../../../../cycle-in-a-graph.md) [vertices](../../../../vertex-graph-theory.md) has one already coloured [parent in a rooted tree](../../../../parent-in-a-rooted-tree.md), leaving exactly $q-1$ choices. The [multiplication principle](../../../../rule-of-product.md) therefore gives

$$
p_G(x)=(x-1)^{n-\ell}p_{C_\ell}(x).
$$

Equivalently, this repeatedly applies the [chromatic polynomial after attaching a leaf](../../../../chromatic-polynomial-after-attaching-a-leaf.md) formula.

To compute the [chromatic polynomial of a cycle](../../../../chromatic-polynomial-of-a-cycle.md), the base case is the [graph triangle](../../../../triangle-in-a-graph.md):

$$
p_{C_3}(x)=x(x-1)(x-2)=(x-1)^3-(x-1).
$$

For $s\geq4$, deleting a [cycle graph](../../../../cycle-graph.md) [edge](../../../../edge-of-a-graph.md) gives a [path graph](../../../../path-graph.md) on $s$ [vertices](../../../../vertex-graph-theory.md), while [edge contraction](../../../../edge-contraction.md) gives $C_{s-1}$. The [chromatic polynomial](../../../../chromatic-polynomial.md) of that [path graph](../../../../path-graph.md) is $x(x-1)^{s-1}$, by choosing the colour of its first [vertex](../../../../vertex-graph-theory.md) and then each successive [vertex](../../../../vertex-graph-theory.md). Hence the [deletion-contraction recurrence for the chromatic polynomial](../../../../deletion-contraction-recurrence-for-the-chromatic-polynomial.md) gives

$$
p_{C_s}(x)=x(x-1)^{s-1}-p_{C_{s-1}}(x).
$$

Using [mathematical induction](../../../../mathematical-induction.md), substitute $p_{C_{s-1}}(x)=(x-1)^{s-1}+(-1)^{s-1}(x-1)$ to obtain

$$
p_{C_s}(x)=(x-1)^s+(-1)^s(x-1).
$$

Multiplying by the factor for the attached [trees](../../../../tree-graph-theory-split.md) proves the [chromatic polynomial of a unicyclic graph](../../../../chromatic-polynomial-of-a-unicyclic-graph.md) formula

$$
\boxed{p_G(x)=(x-1)^n+(-1)^\ell(x-1)^{n-\ell+1}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the graph theory course of the University of Oxford](../../../split.md)
5. [Graph theory course of the University of Oxford](../../../../graph-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
